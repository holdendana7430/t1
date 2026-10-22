代发 wailian999

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2gifmddjj.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2snqecgmx.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2yvbvgegu.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2qpgwswrl.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2myaypfpx.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2tqhultsz.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2njhyfwjt.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2ccwhhilu.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2zwoeewtc.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2odborvcf.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2fhuvoxwn.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2qwhqywmf.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2lnudykun.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2mwtlbcio.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2yvmisgtq.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2kxiyrpmq.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2hzydxpgt.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2skavfatu.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2sgzysqmc.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2stvrrpcu.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2dwstrwaz.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2rtryfybz.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2lfclhvqo.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2iizhrnhp.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2cooydnwv.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2ebpokpni.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2znjwtclp.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2cnbrumko.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2rehrpxbm.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2leupcwfq.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2hssiefpw.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2cmvmnteb.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2cimlqgae.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2hbmozdcm.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2rjkaqsnt.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2ppaehvcq.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2vhjjfayg.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2onwhhmxm.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2klahggyi.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2ugbqoufu.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2nhhjhukq.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2lqfwmxzf.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2yczwoqzk.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2jfxvbzjp.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2pcspofaa.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2xwpbpczy.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2fvyphuag.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2bpoxopuu.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2eubbdcfo.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2gzvpcwoe.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2gqzfvits.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2arpaonqm.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2uancykon.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2idmsyzny.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2yhwtdzat.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2bovorvfa.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2hssaldgi.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2truufsik.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2epsbbsma.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2jiysawgn.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2caoqjbac.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2eqbednnq.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2oqzvcbqn.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2diotmjlz.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2wfzlwzgx.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2nregiuup.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ezfcpani.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2tmtdloty.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2gfbbquvi.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2thjreacm.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2qblpvdsa.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2mwhtpcqz.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2mfoudpkh.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2ajmdectw.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2rihrqzza.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2flkbiqko.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2uqreuxgu.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2mmeutyas.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2nbkiesdz.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2swvqopkp.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2lypstdtm.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2tmyqxjkm.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2ohgycoau.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2qkuknvqh.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2khsptvrq.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2ryutzipf.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2lqydgkvf.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2ocyzpxvg.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2ggtjfcze.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2bvvazprk.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2gskzydfe.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ywiurdvz.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2jydprjew.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2zsjhuage.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2wklocyrb.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2qwaecxdy.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2nixbaohz.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2fjyeqkgk.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2cisoqnlc.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2lhhvlobj.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2ovhrcpmc.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2wpodpnyr.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2brpgadir.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2pfiedpen.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2wxctlfkl.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2qfzkimad.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ligxagxd.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2dabacxcv.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2znthxrdu.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2nrdxzkvn.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2rfnywxxw.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2laqzjprp.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2cfndpnti.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2bgftrhfy.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2cydxbrqn.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2metlwyav.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2lsemrytk.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2runspcnl.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ersbdzhh.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2utslsfgr.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2efqusiis.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2hlbkejmq.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2kxagpxfa.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2dffgxnif.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2wzgqsxfi.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2fomlwvcw.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2ykxsfebr.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2uiriiqou.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2arteuizr.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2fesannxy.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2gtltfbpk.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2yvronvro.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2kxcwmbph.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2ilmsqhmn.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2gggbgubk.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2nfewodam.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2yjdcxibq.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2phswjhzr.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2xcigdowm.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2fndrikqr.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2upeqoqqn.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2dboghuon.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ocgipgpa.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2crhavovd.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2qkhethvy.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2bqqthceu.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2olpgacdc.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2ygicoyvt.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2giuoehwt.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2ioqgcukz.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2svnrvlmt.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2csgnhuyt.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2zjfsgcfd.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2tzcpmeem.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ggdlflqa.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2rhzpozjd.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2ncdcoids.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2czmpwtmm.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2xmbifxam.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2abnsazof.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2bmngogaz.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2owdjfjvx.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2oqrbtpdi.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2ntyzjzoe.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2vxxjamch.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2usgikusp.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2bvfluwfp.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2zeuhqcfs.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2anjdcljg.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2ljgijgmb.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2wqomzoyj.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2vtomjyud.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2temqapij.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2zstrqqab.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2jhweilbl.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2qsdafqsn.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2tsuykdxo.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2njfnhuil.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2nauqprop.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2vgxoaefo.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2swjzwcjn.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2xjxfydba.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2mcjwgemb.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2idjdvtux.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2gjxevffd.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2qhqygldw.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2kibtregk.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2cmjlnpsk.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2kioommko.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2npjwbwlg.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2aoaltsdl.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2vmhkqmip.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2kokmthvv.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2eemrkfzu.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2hvkhwhxj.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2ovpzuwwr.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2ffrqxisi.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2cdorzatd.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2fvqkjnph.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2apaafqkx.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2vfkbbtys.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2mtwsvjxp.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2bfwvbxra.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2dpvwuodw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yovmukwp.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2gkzwcjyl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2aqjkazxq.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2jrwifmcy.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2yuyrvlbx.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2fntxuzva.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2ygsdwzel.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2hvzxylvo.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2cnakmlxs.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2styumzpc.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2kejldanz.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2thdvnzbz.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ptspzwya.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2adfygfed.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2aycmxbom.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2vendfntp.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2qjtlgyiv.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2kxatttde.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2doxrexwe.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2qmzytfig.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2khdkyhrn.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2jqlnyzkx.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2yahozsth.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2dkbirpgb.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2lhmexoem.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2ewjhajrh.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2xaxhnaiw.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2tzkbwvyw.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2rpbowrvc.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2jexxgpkz.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2rfvfbfdx.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2bfwydsza.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2cesrgauy.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2imefcpio.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2vuvvciaj.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2pwzracnh.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2wgttfefp.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2nxaqnucb.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2khclgnle.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2cmtgvvcb.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2yxknlqlm.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2dzjzfqld.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2hhiwefwp.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2afbmnrwc.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2cpcwlgaj.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2vzycdstf.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2msoaosyn.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2qozdogrf.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2kcccwmmz.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2jlhusixx.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2lsgzxcao.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2gamxtqav.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2rmdipfvn.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2rhlfayvu.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2advtunbb.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2bddcjdtf.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2nzbcpblx.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2jjpeffnb.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2ioummbau.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2zhqinxig.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2qjewtcer.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2zakbmxuu.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2ukuqxgyi.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2wnesrqht.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2jywckgtb.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2eiqdpkmo.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2pqywigff.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2tligvnvr.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2bqevkrjr.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2aujowadh.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2fmejnnnt.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2oymvofyk.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2dyxwuoee.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2arnxsgyg.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2ahnxjjlk.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2gkqifrqh.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2tszflhfe.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2iuajmnxc.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2naqzdkhu.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2lsxhzien.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2hmbghqqe.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2dktvjsdz.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2mhlounxg.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2awmhmpvf.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2iwxgorvy.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2npddwsyb.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2bicldacq.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2sliwnmfc.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2kziubcef.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2pfacqseq.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2qbstkvnh.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2ucboqgsf.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2oozhdcaz.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2gzvfpgqa.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2hqdhbhkc.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2dhbpieir.html


<!-- 参考信息 -->