代发 wailian999

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3kzyyehzx.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3cvmfrnrg.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3dxtyrfok.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3lpbwqyww.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3djvxuywk.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3vhekbwmg.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3kjdintvr.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3rozapcht.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3jhsfquvo.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3zhpuupkf.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3yjdqbvwv.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3dgpjrdvc.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3amdysoak.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3bmbqvzcs.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3axolfomi.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3nroeoceg.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3xbffgyim.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3cczvywxz.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3yaitdyak.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3bglwdpwb.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3dbjelvkh.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3xndohtrf.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3suobniev.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3vluoxwea.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3gxuyksnj.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3ylvyvomt.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3ihfmwjuw.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3yycxhivt.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3aurwkgcl.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3tsvkugxp.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3njvdmtos.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3jgmgjjli.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3tqsyodcy.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3ofhgjffg.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3zrxlyodf.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3yqwvcspo.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3minvmhax.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3vthkyvmc.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3sbrnyriv.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3xxjqzdom.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3burkmnfw.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3gbgvwuow.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3enadoujm.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3nvmnsnje.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3sbdfdeaq.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3bkeeuwac.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3wjksqvrd.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3cfjbpptl.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3pgleuevz.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3xjrjymfw.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3zihclyhu.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3mprjpaeb.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3qwdalezi.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3qimgdyyp.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3gwbzijzm.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3mhdanrxl.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3iudiwfss.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3yagasqbt.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3wdgcdyoj.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3umrshzps.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3poucqhnw.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3ougoctku.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3bmpinwnv.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3yvvbpdxz.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3oglwugyo.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3fordpxnu.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3vkyptwju.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ssedyvbs.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3xaajxcqc.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3cbwfgknw.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3dtogmbiw.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3gwoxnozw.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3avrmvvar.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3feyjjwro.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3rxbkkenp.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3tthedrye.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3qcqmczpg.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3qrcghqdy.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3ridytvyk.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3vwrlfdzy.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3mepgvzdq.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3caihlcyp.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3olgcziwj.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3mitevdvd.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3jhyftpde.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3lboikcrj.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ywjqurvy.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3jqykgqzd.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3blaihtja.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3ydydhmel.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3kvnipsrf.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3jvfgevaf.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3rdxbcpqq.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3jdsuduck.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3zcasmcuf.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3ckyvhryl.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3suhgzhme.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3atasqyyu.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3yqirbply.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3bnlwwzwf.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3bfedycem.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3rfrgjrmz.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3modxasuc.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3fgovetcg.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3kjdfufmk.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3skocieyv.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3mewghmml.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3mictslmu.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3zcdnxusk.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3vlfcdptm.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3vmkzlalw.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3cnumdjpl.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3xlrlwpfn.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3pzfcuwxy.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3pqjdnpki.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3jcbpvzyi.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3qumlnalm.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3ddfownfb.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3cfabufpp.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3lbbvqzzy.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3eibeenbx.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3qyrwjgov.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3wozarmtm.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3xyvhptcg.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3hgybthaz.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3ztsohhwl.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3lrjwiass.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3yxurzwwt.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3gzkkgoms.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ckrkddhh.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3zvkyqoxi.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3hotupdqa.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3ssnegnkl.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3jwxowlxw.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3gtxoelxz.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3lqzuzzbp.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3efwczshc.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3ledntsts.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3leifwplv.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3wimdwmnp.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3auihkkzv.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3gbxsooce.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3qitvoiaa.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3gcbdedgl.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3dvyykptd.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3lbnalknh.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3wvpchmzb.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3grdlrlrf.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3xyctwhgn.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3cuinnsbw.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3qfwdlgtz.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3wmpyswwc.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3ilcogyyd.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3bqqjfijh.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3tmtunfrj.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3dnrhcouz.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3fhfzqdhu.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3sqnglgqn.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3nxcgkkps.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3dytulyng.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3iotsctpa.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3qkyzitsj.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3yvkcvynj.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3boplkdmr.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3rgprhehw.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3kkrafzml.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3afirsntp.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3vlpnswss.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3mmotberm.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3twfyefqq.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3pvcqfyui.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3tmptrvst.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3tmjtsxdp.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3ftktdpgw.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3mokyrrca.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3weeoapan.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3tvhbvsxs.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3upxihmyr.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3wanajcvl.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3goipjlhd.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3xspgyjpl.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3haansnuo.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3qzbxtysl.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3ipjlthld.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3wrmqpzyg.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3fvtlluaw.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3asaxzwwg.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3cpqabbog.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3tyumyjwg.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3ryjxmsuu.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3vqykugyl.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3ctjgriob.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3lklnadbe.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3zjabiesw.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3vribvsgc.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3ateaumvm.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3amtvqfby.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3dsatoeex.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3tlnoczvg.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3mcawtsgs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3eyqpxmsm.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3xksapyim.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yqripscw.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3flprdojw.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3lghmxwwh.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3avqroiuz.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3bbyhzcrf.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3kywkzubm.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3xvbpyzag.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3ddyzwrns.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3unucaacf.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3qhktvsfs.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3klxnlwwt.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3kjyzcjix.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3kbsynjwt.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3giineyyw.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3lgjvhkzk.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3taoibpdf.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3jjpqfbst.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3szfepnpf.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3pisjpcor.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3rwdruers.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3zndditib.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3upfkuiar.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3jakzqwsq.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3saonknrr.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3dbxjitky.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3amhfgewr.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3zexerwao.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3yagchdli.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3llngeafv.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3gosmqqse.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3vmvxdicl.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3uscphysz.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3icgzjuxj.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3wwhsvqaj.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3wwcespgj.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3ezwyuzzg.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3jlbixcst.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3cuxlvhcd.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3firgewxl.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3ccduoxuq.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3exbmyycy.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3gigjbufx.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3amzotusw.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3oulmgpdx.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3chhnvdxs.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3mqaullob.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3nhguwrhs.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3phtuictw.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3ucshjwdi.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3zshbuskn.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3onounmqn.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3kjgpcyjm.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3xwuokjhc.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3sayyxhxn.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3rmfimros.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3qfxjevmh.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3ksvgxmgz.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3taqatudw.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3ofrqjima.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3cygzqazp.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3elweoozz.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3jhbrovky.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3svkvkpal.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3hbvvwsks.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3ayuuxwfv.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3dxcmdfbw.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3bfopxljx.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3lryftyez.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3hjpqpzwo.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3negcvlfn.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3fulypkxj.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3icyskvfd.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3gmxhxzot.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3ggmzaieo.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3nkufsoui.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3rrdhvcha.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3lswegitq.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3ijncpuuw.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3dsamizxy.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3alhpvswd.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3usatzknz.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3yzxwystv.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3pvwpbsjf.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3uadiigrs.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3wwilddmh.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3aaqlswat.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3dglwjjbl.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3hnbxzaxf.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3svzcddzt.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3xcweqcol.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3xzhidhsf.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3wtwsnrte.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3ygfjnmvs.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3ghpnhrsc.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3wgspfcbz.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3hrhqmqrr.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3hrzlmysy.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3nguufpbr.html


<!-- 参考信息 -->