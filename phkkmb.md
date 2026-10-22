代发 wailian999

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2dnulwnmw.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2dbsiqkeh.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2uxybzqck.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2cetmfoff.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2lumjkzmk.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2nqvqxbor.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2sfxgqdaq.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2oibfgikm.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2rbozyfhv.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2typwllhi.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2omsnexol.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2fhcnqxfc.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2jytkojib.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2ibwjtipg.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2sjpwwjqk.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2kkvgwsdo.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2zwsjggvg.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2kzbxybsb.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2cmmhyhfq.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2pqsetntr.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2kkmrdacl.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2vxugbuwc.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2wnepvzbh.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2prndgash.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2zmkxvpgw.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2dzjmindv.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2eyrlqqfq.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2steljrpy.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2pzjyzyet.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2eivjszyk.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2zuyrzduo.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2iwwjdqjl.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2kqnkwquc.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2gyhpnxox.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2octzfeya.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2convxugm.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2zlqrysgn.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2ewnxrjey.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2kybrcwvq.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2odqnfzxj.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2umlimlvn.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2bxzmhxlh.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2rvxcvzbm.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2kbrhtqxc.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2okvpwmtw.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2sdvfmowm.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2oudznhen.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2melfyvgb.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2nikejtxh.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2yejiatjt.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2aheedast.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2xktjdlzk.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2rhpmyalk.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2sxnowyof.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2jdxdawph.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2auwtiqvt.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2womepvnc.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2xearzxll.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2wfmviodz.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2tbvthmcn.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2hphvuztt.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2zdfkhncz.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2mdanfvfy.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2nkfsqunm.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2okinqqxe.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2rnfwbtya.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2vqimgssj.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2nbhvgsqp.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2xvkxtglg.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2djpeyppi.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2ibczejdk.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2spopcwox.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2jvzqsskc.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2ejxjhcaw.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2npcxcuki.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2fmedbpxt.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2zksqkiqz.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2ldfipqms.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2rbkixehh.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2zfhmmfrw.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2xhxzksxb.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2njopsqse.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2atkofkff.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2esipcegk.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2kcqxmvse.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2texrsjhx.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2lkdiufvp.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2aqhbejko.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2qiwldbyn.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2acfhvexm.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2innalouw.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2dvhtncrm.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2zgommfoq.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2jvswjfww.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2onymrozu.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2kpvhxqlx.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2qbtezyoc.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2iazlksjh.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2glmdblbk.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2tamukkfm.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2mhfwdzgj.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2zgcigbob.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2xhsyudcq.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2lrjmuork.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2gdyxkjjc.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2kccouhbj.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2isytkjep.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2fgiqvwao.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2mzbsqpuj.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2wurhlmad.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2qtubpxyb.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2cemoietw.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2pkzlvqdr.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2pzbxlbrx.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2qgrviaiz.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2iqzcwmdr.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2vijsqkhd.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2jlwhkvvy.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2gchxebgw.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2cqnpmese.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2idlwherh.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2yzyinsde.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2trymecer.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2skxognaz.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2duimliki.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2irnnirud.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2xyqfdsbt.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2uvnvuuzf.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2uwqdskcb.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2iarslqry.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2kdnpmejw.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2ewanctlz.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2qrlkmerm.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2ivopqtxj.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2uzfokkna.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2embjjxdb.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2lqviitwh.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2uznmoueg.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2gjupvebc.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2qagoudmm.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2iomaymmj.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2ynhwqwon.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2amouqkfr.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2tcsrfiiq.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2agnaehcv.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2hcylobcp.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2orunzyue.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2xasxjweq.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2cbzgkwsb.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2ggxsdkwz.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2qyrkakhy.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2nhrrijmd.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2exsuyuhb.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2oeyzxhkx.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2ohfpmbre.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2zokzhaws.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2gicidkgg.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2svsnzndd.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ybpmfhml.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2nskwrkie.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2qzfahiij.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2eivitdci.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ndkbkovk.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2uftvevtk.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2keqhmpcz.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2flekyifl.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2kpaygqcb.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2ozcjgees.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2iqxkmepv.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2sionqosu.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2fcjlcaab.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2feczhijq.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2iqvkbnzf.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2lcnuzjyw.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2dlphjtlb.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2wnvitvbx.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2zdcrkbps.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2gughzzhs.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2mltqcrag.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2hlqwnzsw.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2vcoemqxq.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2ovtnyszf.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2dtoarsqw.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2qgzmttts.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2syljecub.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2iwlflgkp.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2xsascsmc.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2nggicavk.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2wyrukupx.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2jvgdtwad.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2quphadhs.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2uulvsxya.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2fbchsorh.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2mfrxqqdd.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2fggmahlm.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ravyhwrm.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2zhwioxhd.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2zvpfwyuj.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2hwyjyall.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2aiwmaakh.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2magoppxl.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2wwxmurgq.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2gogniark.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2puoasdwe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2sthpgdsm.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2pfakivvn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tgeypzek.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2iipwrodg.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2pcicrwxt.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2boibweco.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2mdemtnnm.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2ohspzmfk.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2ojosxqjf.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2rklrmrfn.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2adtkpvaw.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2gmpibjrt.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2yajatmrv.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2fjfxzkgw.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2vfbsfchg.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2fsfecrxl.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2ganczuoa.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2qpntfivk.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2tqumejre.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2fdhpiqtn.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2uaztpdzp.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2zmynhncj.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2tjftkply.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2kyvagpep.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2heauggfk.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2dqmcpibn.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2ebqldbwj.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2wbddqpzn.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2pwyjhnde.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2tjupixvp.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2cpnmddwe.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2pfamciza.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2mcfoavos.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2sdtbhncp.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2xjsagoda.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2bdeehyef.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2lxgaynuu.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2snnoebkt.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2gyuofwoc.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2fscuxpno.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2rdzheqma.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2tfontmui.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2xzgezzxf.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2ixjwgqmi.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2voyjpuzd.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2ctvgfcyg.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2idlxdxbi.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2pagxirvs.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2awopwurr.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2iocrcfob.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2yhfpiwsf.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2rotvetzf.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2qcjkuzjf.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2zxtzrhlh.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2kkrykbde.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2xthutwbv.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2exmotbin.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2lztvmpum.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2uamanpxr.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2iltcxqfw.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2livndjyh.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2lcioxplb.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2vpydqusg.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2rxoyvati.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2buftbeic.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2lkjqdqfz.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2sabkusbi.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2iffghdci.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2hxkbhqox.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2kkyxbqas.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2ipitnyro.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2uzvqqokt.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2nppgvzak.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2rcnhmwff.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2kiomfjtl.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2jxbinkkl.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2iweghogq.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2xwvsbwrw.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2lmdgitdl.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2kjfhtazk.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2kelcmaeq.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2ibxofhbu.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2malgpjpl.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2tmevkraq.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2ucztvqey.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2jahgcbar.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2sfcglqcm.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2yrqwceib.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2nbkatiww.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2spsnydwi.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2vtjhggum.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2gzoomkks.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2inlujahy.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2jdbjgodp.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2gokmxxgw.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2kpwmpcsw.html


<!-- 参考信息 -->