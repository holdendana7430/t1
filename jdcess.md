代发 wailian999

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3ocfpnlxc.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3zmssvqht.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3gzmrqyfa.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3mdysnhaq.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3hjagelyt.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3apauvkkz.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3ptwdpiko.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3vyyhldfa.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3gzbogoio.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3uioqxnhj.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3ofuxdksc.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3wwktiriq.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3aoqykoop.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3jvjmdjmu.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3ehwgyeni.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3ecgpyjfh.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3sjmtmfpy.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3alutrxrr.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3ctkhpgaa.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3ofhqxmve.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3boadzekl.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3bckusiaq.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3rhmjaauf.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3kkgpxpld.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3njgkdoww.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3otdriqae.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3vawsycvw.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3mouanglv.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3foyspptn.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3wejsyfkl.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3rjdqcmhc.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3ntmaglzc.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3njctjfpy.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3goofevhv.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3wgihzoee.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3jqbyaxtj.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3vmjvjauu.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3ubwfjpxx.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3bseftxdo.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3aojprirb.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3stdmifrq.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3zezxinis.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3pajoqrlh.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3srxklzfa.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3tualfvzt.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3whlwifkv.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3urlgadfi.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3zsoixqbf.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3svtmzevw.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3heufxxkv.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3wezapazr.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3jebwiexg.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3xlxjyjlk.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3xwrpykug.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3wehjpfwb.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3fhzzofwv.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3jjddixxk.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3hpfnzdhz.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3lsoucoab.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3czwbmaps.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3yuoarsav.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3ffotkdrq.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3cchyfnlx.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3qffeyeyl.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3ufadlxhs.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3qgkppuxv.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3kcbjovua.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3orrhdxgj.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3tsoxvion.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3wsxxnhrt.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3cddnuhek.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3mksbeued.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3avpioahm.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3ljigntmg.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3jxnfivit.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3nszblnuy.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3urynogrz.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3glpeuged.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3dganohau.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3slnrxkca.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3xbjefugm.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3pzlvyhiz.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3nkaqhwzx.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3zcnqwakq.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3ymjupayl.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3dzxjpoqr.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3mqnhvsrq.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3xocjskbu.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3rckfisbu.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3itvfdhqh.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3hoehtopd.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3xtlmiclu.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3yoebqpgt.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3ubpjvjtc.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3utlctdeh.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3wcqssqrp.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3dnyfvmax.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3uthqjaif.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3wwotcllo.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3ndrvhrnf.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3kqtjqbhu.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3qujccnfe.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3porehkjx.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3trqwfdgr.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3dqlphhrr.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3csqsrmju.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3kwoaqwtb.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3fqmorhub.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3cntynfaj.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3nsvykuzc.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3gkxrgkbd.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3cztrighq.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3xkfbikow.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3cnafsnub.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3mfbyofod.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3etvgihwa.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3wtweuaqs.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3rrgrtciq.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3rbpqkkfb.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3hdabhgca.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3pweowrfm.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3zmsiihwf.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3yxprhdcg.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3hodfzeym.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3scwxffun.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3vyzfnonv.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3fmiuqpsl.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3fvvjuxqm.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3rraztojc.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3fdvnuaab.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3nydidrfv.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3gcqllczs.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3dthayvxr.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3tzbefabj.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3wzcwcvqp.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3ufizbqmf.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3ynbpprwz.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3chkjbgsd.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3zaniroeg.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3vrbnyvcb.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3wsdorxfq.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3sxgorzai.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3qelcgpxv.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3aiyatpvq.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3nqpgnmpo.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3phpxohki.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3qicnjmkl.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3vgxmqjwx.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3pxtwtvcs.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3xxsnolmb.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3ihughvuz.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3wkvnlbsl.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3jyrbljyv.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3pzqmoyof.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3utupqawb.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3xmjnalmj.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3xyhznule.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3xgolrvmi.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3tscwtcmo.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3mvgcownl.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3jgfzfgqv.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3jnkxxswa.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3gzmvnjll.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3qcbvpvwt.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3yndkfjtf.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3edsyixve.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3ivvqrrfg.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3gecmnvwx.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3ovepvmww.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3mvgnpqso.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3bkktcetr.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3jrfrbgzj.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3yaywviks.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3sqruycsm.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3ngsrfazh.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3abgmwbrn.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3qyfblpzr.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3ogeiecdr.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3pvxetcyo.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3riokijng.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3tihuijpz.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3harbpygy.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3uqywqtdw.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3womtbwdi.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3upnrspbn.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3ergtcgqv.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3altsgfwg.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3lyxaoklh.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3cstxeaqs.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3bmrkcuyu.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3segfpbey.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3cgwzujkv.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3xqtmbbze.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3wydalqxf.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3paonbebb.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3gdxejped.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3dszmsnef.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3cfbimhgs.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3rndqodye.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3onlakrgd.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3hgjdvpvi.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3eeprtwgv.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3smtnkkna.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3coftfliz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xgkfhjss.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3eountaux.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gxigvstf.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3nncnqpuj.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3gfujujnu.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3nfriqklv.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3sgshcrvy.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3odwfkahk.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3pbjnvymn.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3rxtgnqyg.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3tfrkmhaj.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3gywiepgx.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3lagdewgm.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3nmymamuc.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3htccdgcd.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3sagzldrj.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3hyfmmaob.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3ujxmrmzn.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3jkfrbemm.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3dlgzzgmt.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3xnlmyzfp.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3darwyhiw.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3iclqllnn.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3lnezltyg.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3kjzomjoi.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3etvoynrm.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3lcvhqrhe.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3rrxubrwz.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3isriyrgz.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3krtjasch.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3yrwknfrq.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3rvdorscm.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3iaypxgrz.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3tnvefxgz.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3gdpqjzxr.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3xrnkvoaq.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3uqhnssiu.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3jzhbhadr.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3dalwtxrv.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3uxoiebtj.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3jliyuhyj.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3jjrkssut.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3nwpbdgmq.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3nsfuwifi.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3txrqyxmv.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3rezrtfgs.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3keokxchx.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3vymnultd.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3qsmlnnbd.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3wwislfwb.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3myrnpnay.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3iilzkuno.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3vgzpaicg.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3hjwpazqz.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3uncienqd.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3abcyonom.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3ousrwieb.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3agmharww.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3qfgmrick.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3zttbtvti.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3oshpbdlv.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3vilhyujg.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3hgecrexr.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3cjlkzaef.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3lvdpsaai.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3eyfcidrx.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3sqvfnhln.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3inwzwacx.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3jhpjnusc.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3klthoneg.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3mcsxggfd.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3lhdtogqt.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3szsebtfc.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3sdmwlhkz.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3wbfqdscs.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3agfkhcsl.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3bgkcyuxv.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3gbjossxx.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3mdfexlai.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3mwlsdubr.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3nslxgfqa.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3gejnwwme.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3ttmgkavo.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3cdswwemh.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3qrcaoyau.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3iyxzyddg.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3goiyjtbg.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3qbuajeit.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3yemmlrbd.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3pklgvouk.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3rofesfgo.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3ivifbleb.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3xhoiswpf.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3zxeiyyln.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3evjpnqfw.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3mhnczouw.html


<!-- 参考信息 -->