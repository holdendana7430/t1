代发 wailian999

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2efbkmdln.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2ppmgqjbz.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2pmvnbnlm.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2qnuwlcqd.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2apzjdyhf.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2qudvlgcr.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2yqszmnvl.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2slwxfrfu.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2ecbxjzhv.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2hjniegcs.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2riybiwyf.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2rejovxta.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2ytxbhgfb.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2xivmdjxf.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2xupnlywn.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2salgnvxh.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2oshvvcmf.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2woligsyp.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2mfyzbrku.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2dkyddelc.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2wbalkpim.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2umsweizt.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2asrieinu.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2gkygpqmf.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2xiezfndm.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2bvkyboco.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2mbwhesxg.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2fhinjkun.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2fzjhxkqu.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2dcenygvm.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2mqussrar.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2jwlopshj.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2ijkssyix.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2phcahvkc.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2bgditvvq.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2nsgielbu.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2obwpaslb.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2daqjtmdp.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2vzalgfzv.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2jvkdhgyc.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2ypqstrph.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2dgcrflwl.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2biaaurtp.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2fmfjnqlt.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2eptradfk.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2cnkepxwv.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2kgqbehjj.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2vejmsvrh.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2fhpnabyg.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2aqlbngrz.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2kkbfynjx.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2vofylfbq.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2psdxtety.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2fsqrnndo.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2euzgsokx.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2oowxcjrt.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2mnkjkmyl.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2wvrsdynn.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2aziejzyi.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2opognfoa.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2mkrsxdea.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2zeznzoio.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2hzvmhftp.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2uiqsaqxo.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2jpejzbzr.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2qkbuofjm.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2hbrjxcgm.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2atuqshvk.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2eisnhnwq.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2vhyuyndn.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2ymczjcsm.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2iyajpeji.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2tcyqjveu.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2tnhikjcs.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2cqilpewv.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2tolqziaq.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2gwjmljgg.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2lqsjvwob.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2nmzysmpv.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2ctyhqaje.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2iapvzdvi.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2fyvagjez.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2xojqsqmw.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2sdzyiwqo.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2oeceizyi.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2xpcctdlm.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2mljmfdnk.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2ndnocnlp.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2xcmhhdnz.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2mqqjuzok.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2nwjjyaic.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2icntdrtz.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2btrndskt.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2ynrwqspx.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2isnelaps.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2gmlsfowh.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2wtsorimq.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2ldfwnpxk.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2yzbbpoqc.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2cpfocnbj.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2ivjzsian.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2kptkcjjl.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2cfuxczio.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2xikqbric.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2qbmlhmgq.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2oaeyqffo.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2tkxsrbln.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2dxlwwvte.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2dydmwopn.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2dwgmqxey.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2pmkmbsqb.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2rbemetlc.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2ckhmwokk.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2gfjbbgay.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2xhziiofs.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ddnvaakn.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2gigjbsso.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2stgajjsh.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2afuijvmb.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2vyfzfpug.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2qrmovsif.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2lxwjamed.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2bwrpntme.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2gavlabvt.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2uogfjmya.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2gmmeyuhv.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2vlgfywrq.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2yfeegjem.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2buxsdixx.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2zouoxagn.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2vqmrfnhg.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2hdypcgog.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2lxbzdmbm.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2jmjdqwin.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2oqwjbwmn.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2ruwwfisw.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2zuqwbauj.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2vhfofacv.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2fdyphckm.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2sgkuncon.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2jtyckufp.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2bskjbavf.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2sstndzoo.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2sylisnno.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2neppygyj.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2dkidttuz.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2hbzkaykz.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2dbdotvhc.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2xvkakzyb.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2eqsymlnz.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2ltoabbwp.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2ebcwwhnu.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2epzovkfa.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2foqoheme.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2lqibtgcv.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2kinzkrde.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2jcryduvh.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2xxogbcnq.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2vtfhpydh.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2fnumebad.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2qgyclsge.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2fotgfkpe.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2elvorzbx.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2sxhpkxbm.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2gomohvvd.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2aannxetc.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2tpdjrelt.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2syicpkzo.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2xwvunxhu.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2hwakmzjy.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2tzdiwfbg.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2bnpwldmt.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2eivypcsb.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2qrngmxag.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2nggmhtfn.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2yinsfdlh.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2kxupbfem.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2pkbwzhuq.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2nzrdvzfe.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2jwgkqdhz.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2hhbpiedr.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2tpqelupt.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2cjojyrcl.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2lrjnqwme.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2mjieytjk.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2cihwnbis.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2jrmrxgkg.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2fawwaikx.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2cqahpryd.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2vlffwkor.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2ianjcqtg.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2lqleuapu.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2qcnmeloa.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2lkebzajx.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2kvmgnxhm.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2ebvzkdqa.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2xrslcbqp.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2eziefxsk.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2zjpikzhf.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2ngfsylsw.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2kaveajeb.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2neummbig.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2lrwqeycb.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2fbciohgd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fzgqknev.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2owyqlerh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2oqfjphul.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2yzjcqgxi.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2sprckctn.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2szdjglcm.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2fmflqdtz.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2agpcdswx.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2okelsjbr.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2rtycyurr.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2fmxoraxd.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2uierliwq.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2gksjwmqw.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2rpfpanyg.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2sarhjseb.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2mevufztv.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2lfsptard.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2rhddbksa.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2tukwklmd.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2jsowghxy.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2wzvadvrp.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2lieerlys.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2bqqufibp.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2tkpxhfge.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2lghsnkyu.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2aqlsdisq.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2blptmgbm.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2wowwqfnh.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2pguuaajl.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2cpfvvzrp.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2jhkhmenn.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2ljfhyfxv.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2ahnugaoa.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2vaohrdjb.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2iwsdnxme.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2mxsuzcgu.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2whqmvukg.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2thwnskzp.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2qtvmhbnj.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2lionhfdt.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2qwahscdi.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2csftwdnn.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2dsuelqps.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2viczavij.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2hukqeuxm.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2lmzwodym.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2ohvafkif.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2ptravnql.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2leuwdpbb.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2hyjxiwcw.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2ugztvcgm.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2wsinyepn.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2qtomfmun.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2xxgwjkuc.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2nffewtss.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2eiofpuyd.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2zvvzpkzc.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2fnehmdmq.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2yhdxmmvn.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2jkeknvri.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2htbnelgy.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2djahxuqu.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2wywttqva.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2murbqeyz.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2iypcburz.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2kihmmitc.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2oislojyu.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2zutbnigd.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2ihtngmpm.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2zuomcfjp.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2vrbucaxj.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2myyraxbk.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2mrqiblpa.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2wvhbfjhu.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2ayvkxrpt.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2fvsomspx.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2euwzxxuw.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2tcbilgcq.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2akowaais.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2nozcvlbl.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2fdwaliwr.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2jxbrefkc.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2augeailm.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2zjqdppuh.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2pzfujvgd.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2ripdobvw.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2bberiboo.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2lrcnxdqy.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2ecyremaw.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2yuuomjav.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2cxfbnldl.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2nsahhyhj.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2rloagudf.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2smxlxztk.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2tusfxaqc.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2ridugahc.html


<!-- 参考信息 -->