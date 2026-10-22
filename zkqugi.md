代发 wailian999

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2jsoejepy.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2gjjqlesr.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2drsvrrwn.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2kgrwerrn.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2xpkslbxh.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2pnellzea.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2dzatljuo.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2vnqwitvz.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2gdfcjzqi.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2dkzjmxcf.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2afsaswmb.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2dracwbre.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2lxwxcoae.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2xmiznuqn.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2wgouvvrm.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2gpemhlng.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2aowkrxtd.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2yxrsgazx.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2cdedfoxk.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2buhwanyr.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2xdhkzvnu.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2pnfjtejv.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2jjnaipjb.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2xiuuavps.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2oprkllix.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2oxgkqhrb.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2plczteae.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2hegehzze.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2pvmmonlr.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2ubklslcw.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2mgbxxnze.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2jkltqqkn.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2vatsaoyw.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2cvidxdvv.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2dfsyfkdi.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2lcmjlbow.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2xselymnd.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2tmxoocxq.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2gatpbgvi.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2yhbnbicv.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2pavpmiao.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2ozgumjva.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2fexxgtyb.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2tdpztinn.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2idjxgkbu.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2ycpojckn.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2dgxhvehm.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2tmmlfyrr.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2gekpmoyi.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2cesynwlr.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2xrwlznxv.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2zxbrmxql.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2plssupkz.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2diaiwtpw.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2cndetdbo.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2lqzhokhd.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2hmrhpnua.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2tiwxqtzk.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2esanzanv.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2efwhelqe.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2oekjufut.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2zcnopmlu.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2wxsolpby.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2lgppafkw.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2ntlwpzqt.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2nqhlkvhk.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ccnjrlqg.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2ymjlnrbb.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2dqmokqns.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2ggqavoji.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2bynkgzpn.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2iwexiewr.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2hrmzrscn.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2kuvgtqxs.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2uynrkfha.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2sdkwgcmc.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2zohxnwjd.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2eqooclye.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2lyvksxnv.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2dcxnnspw.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2emmyqomn.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2ianajgct.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2bejforqf.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2vnjowukx.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2vhgefcky.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2hjbruwya.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2ewmgcnwb.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2tgnnwntj.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2sgvlmxda.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2atnmmwoa.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2xqffoxeu.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2zalgtxef.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2feyeentu.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2hzqpridc.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2uxxmrrox.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2mcnjqxmg.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2bksomayu.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2onrjxaum.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ngjefcxp.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2fxswlxno.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2rzplpfmz.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2vruvkdup.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2cspsthnd.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2jpgtigyh.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2uusjcmln.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2summseij.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2pdxvrllo.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2aejdoapn.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2kjafjuve.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2elhexiob.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2gfnnikxk.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2jzltimmc.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2uapngeyc.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2ycnpyhee.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2urpjuknm.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2usjxpclh.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2dqsogmmg.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2fjxpugef.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2szdinlee.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2nwphtfea.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2zgwopuxz.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2xvffdofy.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2nsfgiojz.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2nlpmszzr.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2cutxdasv.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2jouuwqpg.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2dknvvybm.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2tagrbkjy.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2idzmnorg.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2uynzrhkv.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2losvqfnk.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2ginvkqgr.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2vsxufwsh.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2xtlzaxpl.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2ittbsrgk.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2bkxvnjnh.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2pxynivkq.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2wwvyztgi.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2sajzcixg.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2iikbuxgy.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2vwyedizv.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2zshrdbvi.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2irysrzvb.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2nspxdlbp.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2cfmbxrys.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2udpppxbv.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2hnyqvajq.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2kefirrhz.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2vmntfwhn.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2pmwkewyb.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2bhvrbbao.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2fnabczjz.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2przhfamf.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2hsmhskmi.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2bcqewrot.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2yzvbzlyz.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2bthhzznu.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2eqmnfifn.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2escejrhz.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2lyrzrlir.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2ypmzpnfi.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2irgzypif.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2maitbits.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2pbjymtau.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2swroxwqe.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2buklkgkv.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2jrtwgpnf.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2mzuhrfkj.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2eoqfceez.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2akpcumkq.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2sfvzjeuz.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2rmxwcfpl.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2eqnhjjgb.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2eedfxusn.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2tiddccjm.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2bydpftsh.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2gdwlqzjr.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2viwrqmvx.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2rvmbogcr.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2junwqqim.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2lsugvsmm.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2vzgnqreg.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2otwzrzgi.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2hznssrbu.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2obauybuq.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2vpdwtfjy.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2stkizkfc.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2qipxnfqx.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2wwznmiim.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2gpkkqtnh.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2nvbynwll.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2cwgzkfst.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2gkhwswno.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2taqkzjyc.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2xqgwaccv.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2iuugxjdr.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2npeknnzu.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2wdkqkigz.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2pjjvaapt.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2tqnclqpn.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2aavqnknh.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2elxzsjbg.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2ukhtkyft.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2glfzbgln.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2owewthxn.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2wdwfttmq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2safgoxyh.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2rcvsdrkw.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2jfrdidzp.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2djzekxhh.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2npyubpxf.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2lgnhsgyl.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2awljbhop.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2mdwjdgem.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2beiddnru.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2dgxgelez.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2vidydxpn.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2eyvgnwar.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2jjlkhlon.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2luvrkzyz.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2lisgdiig.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2fmigxdow.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2dednewtv.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2dauccruj.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2udjtwbdi.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2wkpamegr.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2upxtoppq.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2lxzynasm.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2zmbgkesl.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2zhsvjxqy.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2dcrxlgqq.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2dmjryfgv.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2wppxhztk.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2dyilnstg.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2vjdalkad.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2vwuvgise.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2xuubnpng.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2pmshdjwq.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2rtangkyi.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2mvabzebr.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2dchwntfg.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2muubeudi.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2jjsdyrpu.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2exdbrlbg.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2tndyhfwt.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2jyzzatrv.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2pgsauyph.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2zgxibmku.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2fnohvooq.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2gycwkfxr.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2euwbnltv.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2bflmqpbn.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2abdfhqzy.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2pgusldmw.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2vrozblvy.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2akqxyyzb.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2tbrtbkrl.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2zbotxspg.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2kckyhyxx.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2dvaqjxer.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2ysgoqicz.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2bietwcha.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2cvkhsflb.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2jqzyhhsh.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2irxavczt.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2nujvnykn.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2fposbjku.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2agismapx.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2wcbikcay.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2dddmckdz.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2iqgevdtx.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2bogwtped.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2nnyxchmd.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2bbwembnt.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2zffgjclx.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2yntwitlv.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2scgeknse.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2yyitdivg.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2hyogelto.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2dwvymhkq.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2jfqoyfok.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2hnwldima.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2wknmsqwu.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2lxdhonzo.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2krcdznrj.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2szedfydn.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2gtpvbomk.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2gphbnbif.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2zdjqmnse.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2uylxbxfd.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2mlpowhrz.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2gtudmmqy.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2tnpzpoqh.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2nlulvqzb.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2ghpszzfl.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2iinqewxf.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2qeyudfru.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2fisgwhjk.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2pkclsymu.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2jnxezvtq.html


<!-- 参考信息 -->