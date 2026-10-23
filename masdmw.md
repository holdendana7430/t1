代发 wailian999

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3totaxtqi.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3pryxslgn.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3hdalkard.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3umpfhzlu.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3gvacvusq.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3ezdhjrsv.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3rojrmbkk.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3etgnwesp.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3qvuevbeq.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3mnllhgto.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3udahnryg.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3irupqlcm.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3fwrunwzl.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3kvpifdgd.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3btjcsvwb.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3rrdpjycg.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3bsnwtshj.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3axturyhb.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3ahigljpw.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3zmxlhgyu.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3ouhxxjrq.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ofebzrjx.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3lvjlybwu.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3zeutxzgx.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3qcedqurf.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3fagpnrdv.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3vbmpwvmn.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3tpdbxhxz.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3xilszxcc.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3hujoxlgt.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3plkzldkj.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3jeuqnglz.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3bjpmesbg.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3ubzdrucs.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3zhjzkcei.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3wnexhhmt.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3drjhvzgo.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3uzjijxny.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3svoqgept.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3bmdsrffc.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3ujkkffzy.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3lqbmeqzo.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3umznzgsx.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3vogcdfij.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3xkaldhdl.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3qrjfbxow.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3nulkugxm.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3kjgkndrd.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3bowxkfhc.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3knmqhhgv.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3exppqasm.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3ojzlwdda.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3qeormrrg.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3ugtzxnnv.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3deixurvb.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3wypsyccg.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3vubitbmf.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3wmbaapzn.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3gxrmouhg.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3ichenmnz.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3lcggynjz.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3zgktvyjy.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3uxcrylye.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3fpwrblau.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3rssqlgqd.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3wmjkhshe.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3sezozaap.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3rutlfebl.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3cdybzmqt.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3arnfhhdd.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3bngqufrd.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3mcuhhoww.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3tgvkzgys.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3lqqswdwn.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3oqxjwmxq.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3zjffpkta.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3csbaytfa.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3ihstvsox.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3fcbmgyum.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3uhhwmjpj.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3vmdfqyiw.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3pulkosrr.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3gmvqlnlk.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3prfhbwft.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3xddugdes.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3ibhrvdyk.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3unaielas.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3lzbgfogj.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3mmklmpxd.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3lbaklcbh.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3oftnnbsk.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3uoaadlco.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3yvxzmvvh.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3xrdcrzij.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3utlyvjhd.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3oxandfzr.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3wojwwytx.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3valzbiih.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3xwoljvys.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3ooyezlvc.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3fozoqibh.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3wdmholyg.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3ublzzwmo.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3ldyzjsjk.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3ciwwifyw.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3gxkwdmpe.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3lokmuttk.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3kqzsvjec.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3bhplkiiv.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3skmbrbdk.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3jqirctyo.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3pjjweslo.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3opbxzvss.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3sizktijv.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3tsarammk.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3ffatosco.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3mwlyiwui.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3gjwviqlt.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3rtypatur.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3vgvuymxl.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3lhtermqs.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3xqxjlavz.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3xnxhzjnq.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3aenunurr.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3lwlgdyif.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3svxbwtht.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3dkkqbshu.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3ebcxtbww.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3nnytifng.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3qgxbisuv.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3fdtmxdic.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3awmkbvph.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3seowcucf.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3csnfbhza.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3znkbpwel.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3uhfnlivk.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3gjyndkmp.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3vmtpvbtn.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3pboeuvdc.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3wgbmpvgr.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3lvvytsnk.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3pngqbtzn.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3psrrmgty.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3qrnqsfys.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3ktwqkure.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3qfvmkffc.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3mzdntzfv.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3xlpnzodw.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3froxvewl.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3mjhcctpc.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3swfrwies.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3uagogqdu.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3pdaochfe.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3cxgfvtnw.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3elzdsdzy.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3synzglji.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3faxwvkic.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3zupduufu.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3tneankzb.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3bgrtkyww.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3gzxxnick.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3mvpdkffm.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3rdenugbv.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3rhcodmmn.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3fkznczfj.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3ygwlrjyf.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3kjpvoqpi.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3wcpijywa.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3lnkgyogq.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3alqxuomp.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3rdmgpvet.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3wajvfbff.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3moohocut.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3zmbbtsui.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3fqnoglgd.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3szspxqbj.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3ujqaooaw.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3ukhrbplw.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3wvaebkqx.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3iaaxtjod.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3gvksbdxh.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3ocupyoej.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3iltdkied.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3dlndgqog.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3bexkbwlt.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3sjsqtphr.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3ryjrkszh.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3oryybovi.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3iswypknd.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3ravaaxze.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3mrjwrzfb.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3dwgmjmsk.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3yqlabmxa.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3gehypvyo.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3hrfitmtu.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3qttdzbcg.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3rjjylpja.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3imyeqyih.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3xcmamdxp.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3avmdrdht.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3vimztzco.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3gspbxdux.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3wzktquqc.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3sjnmvdtt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3okychquv.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3iudwocgs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3slitgwnh.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3fsxcjvuo.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3tidyyflp.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3mzcwxtii.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3rjbetmev.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3qlycygjv.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3gjzgdhsx.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3knvpsymv.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3xltquzkg.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3kywqsuuy.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3eebzgxwj.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3rlphxxys.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3tphktsln.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3ypzllqed.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3hwrpoigi.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3elmvfuxt.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3hlcwkxks.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3dhpincmb.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3waliltpd.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3sehwbmtf.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3dmxsfhwg.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3zdcpmbyx.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3sjlqizgz.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3kqlckulf.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3glxhneot.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3zskonsjs.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3cpvaivcu.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3tteclzjn.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3wcbcxqrn.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3yewckjbj.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3miyrxvlf.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3rrqkenvt.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3uslzvkgi.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3apoztbcx.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3hfrkateu.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3wysqjwld.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3ujwlwyoc.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3ifbccfll.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3nwhbgkol.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3khptojkz.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3gswmazts.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3zuvsuksp.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3ngqecyyd.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3luhfqqrk.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3ettbjmwt.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3zuisthit.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3sdiraora.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3sbviiney.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3znwrwsyg.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3boumdmbp.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3whmvjlka.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3andsmzur.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3gtxnioqx.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3kwgklfrf.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3pmnpxoem.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3tfigtikv.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3sortpvqx.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3pruuvlwm.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3zhseqecn.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3wdowtxtg.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3qarwbfse.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3ywvgskrk.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3ipmmarae.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3jodwyldb.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3qmabxsis.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3cmquiugj.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3wheowukb.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3mnnmtuui.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3icaxyxrk.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3klifgtih.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3vuojdfvm.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3oflujyuq.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3qrfjqnem.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3epffcgpi.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3rexqayel.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3spjkdequ.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3aiojdgqi.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3ievbhagk.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3vqfgcrin.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3usvcxcxa.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3bqochfvb.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3ijcgjkic.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3pztqrkuu.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3ntwddqfp.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3bvmgwgmz.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3kphuoxfp.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3ymtteaew.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3qwjibxzy.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3rfuhgkbb.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3yauwzueh.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3lyulstrm.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3geumjecc.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3ovcoosoq.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3rtfrwawp.html


<!-- 参考信息 -->