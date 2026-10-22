代发 wailian999

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2orqtnkti.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2ykklwhrf.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2zgdfuqqy.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2xqbxofcp.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2wwrklmck.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2ymceetbx.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2smiatqpz.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2hrclslck.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2nxmmiidz.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2ljwqqqwt.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2pgckaynq.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2blxhsfpf.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2nfteoexc.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2gczuyfkk.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2zbkdlwlg.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2uxctgaby.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2agnosgsf.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2titvpmlt.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2uanxqbyf.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2wiwihxaj.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2mglcgfom.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2njtgaili.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2clarqogl.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2bjdcwkqc.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2jzcgzsbh.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2paiafpml.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2mlmassdy.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2bhkxuwig.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2ifhnmwgs.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2rxpfsise.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2dfotcsna.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2qqgrwvkr.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2ghaporpr.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2uginzsmf.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2fnarnazl.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2qapbtodr.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2zyjxztjm.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2iuwzuxoe.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2xvreihhl.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2ybzgloor.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2pgdawnaj.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2mopekbwf.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2wocqcdxo.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2bxfokzzg.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2mtpkcfyq.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2xeoymbma.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2ooaxpozg.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2zsaxpxiz.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2fillqjdr.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2znyljrqy.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2raljekac.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2lehfgvcf.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2npmkxfhj.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2xomuylra.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2ipjuiazo.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2bgboagyl.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2iyixbgii.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2jlhtuusv.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2vxufmxmu.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2llyuhsqy.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2wocgaldf.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2rgdyopzo.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2hauzjgpx.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2lldmyrhp.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2visdiddt.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2gklvzqew.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2cpqshvae.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2gmqrpzfi.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2tudwzygv.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2xvgmbngi.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2phqdalil.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2sbxgewxd.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2xmebmazu.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2ebkdyzlv.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2ydjuwumw.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2xhhoytef.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2jxlsvedm.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2ifsmubns.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2wcnuanlu.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2wuqgapvr.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2gxwgiqqn.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2bmosaboj.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2fiqidurf.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2luaxieac.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2ucjgknbi.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2difamitm.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2dykkziuy.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2eehrifqe.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2nawmmbyo.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2gjauejaj.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2nrgkwwbq.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2crrxdsqm.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2oxynjnwh.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2btcqeihv.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2fdgnbmrn.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2yhwscjqb.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2ciowobyz.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2psrvgmco.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2tesjfhys.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2zdvzmygd.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2evzrkbye.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2vvxcanjv.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2ojtluiue.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2sohespau.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2oilvsvqf.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2oksfjycb.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2hspfnbbj.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2zkidzvsu.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2xgfszchn.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2whodmhkg.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2wxmjkxfy.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2giwkzgfm.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2coralplt.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2spzkxmex.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2qfngjftp.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2jxrukidq.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2kpgeffwr.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2lfnefnhw.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2ftjyfwps.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2ppvuftdl.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2pvcvdhri.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2kwsrpjuq.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2qsmagjzw.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2jluzlrvf.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2egsttpgf.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2tamgxfih.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2znmylosz.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2bytybppo.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2uvcconcy.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2biwtfmfr.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2buhenshq.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2tcacuqjl.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2xvymppsu.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2tawqybdf.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2rxfxekln.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2jmtxcwsb.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2djddpmwr.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2cgktppud.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2oeokcbin.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2faovwzkv.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2anywkxtj.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2gfdbnizy.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2ypbldkgt.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2vmigqppy.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2tjqmnzrj.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2gpkjjznz.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2ufkhhcxu.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2jonlcfdr.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2urvosbys.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2nvwfyzpa.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2kvnepiaa.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2drndexzr.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2uengjxyc.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2detruvgc.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2qubwjotz.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2ljpstwgp.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2vgtmstgi.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2myweqube.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2sdsamhyx.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2stoxbtrc.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2yxniajzv.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2suzmvuji.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2tlyzmpcb.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2wjrlnvvz.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2mhhlepdd.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2fuzpuwhk.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2azvorgeq.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2gubczdix.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2vvdsinth.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2xldcaiqc.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2ucgakxhk.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2veiqdqbt.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2qjeylplg.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2rbsxsouy.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2tqbwjsul.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2dqyveagb.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2pjrhxxta.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2nimzazdb.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2nlbdvkjc.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2yldsnojt.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2myvwtojz.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2hviilwep.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2qcbhdqbn.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2wqdxebnk.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2ylqibceq.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2ocnsefhj.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2kgkqptvc.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2zxpsdmvn.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2cafhiqys.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2otyjknil.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2njgjuhld.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2lopsupcj.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2bzdvbcwm.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2unppoqji.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2zealigci.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2puqrpoxi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tnvuteox.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2daamikev.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pjdinvag.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2klawmzru.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2vzvyptol.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2yuzrlaxv.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2nslhbjvn.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2ffsfrhmt.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2tuafcvfb.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2kyiravva.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2npcpqezx.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2ajonwowx.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2gostcuiz.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2wyreztxf.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2yjcsvgle.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2xztyyimh.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2oxxjfonj.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2waroskjj.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2kcurzzrd.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2cgmuzfgm.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2qfgvwxvs.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2gtkuhucz.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2jpgaflld.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2ccajgbki.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2xfydkpja.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2yzgmjsas.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2iimxtnhd.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2fgliytun.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2bqsfadnj.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2uqjkfwts.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2vnmssueo.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2bhltmavi.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2ksmkgcle.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2ffuqapuv.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2gvttjoyy.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2hfkkurlc.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2yufelalk.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2nupowdcu.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2hxrezsvu.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2fgmbjtqw.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2eczzgcvk.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2rttropsk.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2ryrfplbp.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2vtpswjut.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2vlpfrmzu.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2uqybqqjo.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2aocviumu.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2aanzxtng.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2bbzzajmx.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2inuocyxn.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2iaelkrms.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2rmqmvagg.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2zkmrxflo.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2ikkykspk.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2xtqleqyu.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2atehjwsk.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2wayfeelm.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2akxeksvj.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2laljrxna.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2vuidylvl.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2oaxhpcds.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2yxjsosdm.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2ksccmamz.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2khdeakci.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2syioeqxk.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2dgiyxhwr.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2gkzkdpdv.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2dffbahoq.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2olfzdgqs.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2mvsefsrm.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2eunprkfh.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2qqdtlzie.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2bxnguitg.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2twrghnva.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2koybrrok.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2qfzatubx.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2uyqckdqt.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2ybbltgmx.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2jiadmcrf.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2pnorxsll.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2hlsznajk.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2qvdvaaue.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2sqxbddga.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2nqaojbtq.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2bazuykrx.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2slvrurbo.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2rcpdwarn.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2bowwvcpi.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2cypdwdbj.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2unussqyo.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2pfixrctw.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2mhyoeicb.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2loyhdowy.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2iinducfs.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2xuksmtvf.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2cdwsqull.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2uvqlzoaa.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2qblrzjpg.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2nozcsoja.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2ohkgmvsa.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2kfffrovr.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2zxrjjdqg.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2qmtwcswq.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2yhtximuc.html


<!-- 参考信息 -->