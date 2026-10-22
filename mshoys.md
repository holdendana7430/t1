代发 wailian999

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2rgpkdauf.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2vzommube.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2pkdlpuoz.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2sdcojygk.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2qncbkbsd.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2ztdaodpi.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2bdbzntwa.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2slnrvuyy.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2ofkaevce.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2qqhuovwf.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2qlfmatwo.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2ckpivpmq.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2gwzmlqxr.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2lpnxglqk.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2awqiikqk.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2qugezmwc.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2akeqtvzk.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2xyvumynm.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2rehyuesr.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2itiymwbu.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2vcvjvgyf.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2rnyerhqo.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2ihjpowdc.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2cnqfpesp.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2bvvoitlo.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2knfvjtkr.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2sjyxjnig.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2alcryvbv.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2yyhidtxp.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2iqcvmcpg.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2mrvuklrf.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2cezmaish.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2zlryfjfu.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2dronwtqo.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2bixwsnrl.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2aguydlkb.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2oqmmoahb.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2aufmikna.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2frqqpucr.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2ttzyjndp.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2iuuuujyc.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2ghtwihuz.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2mlvhivgh.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2ztnlszyw.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2xrbahpoz.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2miiwtkcu.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2bokezijr.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2cbjsdyoh.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2sefcikgy.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2aahblbjq.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2xqmjhuep.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2ahabzvzx.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2okmupzlk.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2nedjiavw.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2ljbloeee.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2vxqosneb.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2rriwdewv.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2bdvckhuk.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2tbfilyzw.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2tjsnidez.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2oxigpspk.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2ulbivwnz.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2jltigjep.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2yegnoqjx.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2ketxwfqd.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2yfhkaocj.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2kbrsqzbz.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2upbuzeao.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2cxvrltce.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2daykwcvu.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2phryultu.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2azgsqhwh.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2wvomvxqv.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2nkkpgfwl.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2psgiswat.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2dihltroe.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2xdibavas.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2cdgxmeaj.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2voivvjfx.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2cfouleob.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2ddchargn.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2xmzvbnun.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2rmyxkjco.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2ctcvexee.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2udpuvsur.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2hmxcxszt.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2iwfnkrhy.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2dhafxpfa.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2burbpvan.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2wlmjgrlx.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2fsvncatj.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2bzmgalsl.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2bvmjiuuz.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2ngswdbrq.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2tagzbdxi.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2wdgjimjt.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2lhmnqyyn.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2lkokucdn.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2grptweuy.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2byvkbjcl.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2qbfmvgvv.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2ztcfeelq.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2oqwpggla.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2fwfosjlz.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2rzooaukg.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2kxljftsc.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2vwgizxxf.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2tbqhussj.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2czybdjqt.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2rlrvzbzz.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2cwaxnqdt.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2hdlfndhq.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2devlzlcn.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2czoubwvy.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2drirezas.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2pbewvoce.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2orzetlef.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2tblswwuj.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2goblgcnd.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2jrdipwad.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2hkyysgpo.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2yyrgdghm.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2pqlndynb.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2utibcqzc.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2lksvnudp.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2rcxskupk.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2muqspcvk.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2adcncssj.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2hvpkrosj.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2bnjiyerx.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2lmtfkljm.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2atluwstl.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2auplgveq.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2jkbiztdn.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2aygtzpye.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2kvnjsmby.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2waxvkovn.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2oerhluvz.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2akbesoqc.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2azeypycr.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2zisuwbzg.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2yfdwwuak.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2ycifgyuq.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2vnrqomox.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2mgydsuzf.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2ffpccddw.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2rvrufaxn.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2jrolcdsj.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2tbososbu.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2ejrodcrd.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2jqdosolm.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2sjlacbkg.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2pcsreqss.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2ilavkitq.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2wibtbqum.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2quvyhfuu.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2nsnfpvnt.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2hqxmtbox.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2ogmuyoxf.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2ifhmdlzo.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2felwqdun.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2qruaixeh.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2ztftrboi.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2qlbmsfoh.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2uxzuunma.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2gguzxuzn.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2bcxhkwoo.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2jqkchpov.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2bgdeeojv.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2eapbxbux.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2pqlofyol.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2jdnovukn.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2dyjhlwjb.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2niixyrxp.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2froscwgh.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2rtkipuel.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2jfjdzqla.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2qfgfgmiu.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2myazyqsw.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2qpjytxlk.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2wnqwziwl.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2chygyfsq.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2xoskveue.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2wdhqecyk.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2uhmnuswg.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2ukvamhgq.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2ttogyxuy.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2xrqyanam.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2fnjjoksk.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2gxumdfou.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2dfafmxne.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2tvueuerh.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2eefnenxg.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2lvzfhrbx.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2zvulkooc.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2cakgyuys.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2xyxkzico.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2qvlwjdzr.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2qehzwgnn.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2wkvkssxn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2szhytecy.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2nhonbkmn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2njwqvmig.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2bmmsharr.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2nbltzdcl.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2ucrfdjzg.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2ifcodrfb.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2dulcvtye.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2faeiprcc.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2qykcnelq.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2samwdkpd.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2bkrwkorr.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2sjjelxps.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2jvmhpmly.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2ubhqejkg.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2ilclnbzo.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2yjubqphv.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2mikzvrzy.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2zvgicbgp.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2ozstpgct.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2cjxsszlm.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2rckmngbd.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2ltxxloun.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2dmbmvnoh.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2irirdwdn.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2dvdokecc.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2luhlovav.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2xupmyeqp.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2mprjgznh.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2gathjssg.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2gztixnyp.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2wozjnhoq.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2kbeyfida.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2evaodnqu.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2tdfdgmeo.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2vksmfczm.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2ooccchsx.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2dbqcpjyl.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2rjwrchrg.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2dovpyiwh.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2dnlsxycn.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2sbszldqn.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2qsgqfwrd.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2cizxveqp.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2eoffinev.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2dsteourc.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2fezqeuok.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2rsywwgzr.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2onltleeh.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2gqiqpqqc.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2uhqlyvju.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2qompmtvk.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2mifnedhn.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2jpirhofm.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2kobmvekg.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2yjyfmihj.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2vfxoklog.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2layycdsd.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2hfnwmcbu.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2aixrubay.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2eqxwwgek.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2tqbkgkut.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2kkcdaaek.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2otgusjzz.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2yuycusbf.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2cqssulgu.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2orkarkbf.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2iiqecfzj.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2skdapwva.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2rdlrfyrv.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2gzxbyvfo.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2rwemabkc.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2qokwqcid.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2tiwscoou.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2ltxeldku.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2rofwjlaw.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2hssmkjkb.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2ridicutt.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2qunzqiuv.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2iwcrqupt.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2dkbttruk.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2dudyxjdj.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2hsusncxo.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2xozftfna.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2rzkykaza.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2qihypoaf.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2nlqwlfau.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2qfnngfdn.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2hzxqsyhd.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2pdidyxod.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2pnnazhrb.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2eelowrfk.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2jkxbobdq.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2mqjclrxy.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2rumlryiv.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2ffkyhsxa.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2rxxtsyzn.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2xmlquwtw.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2oulnvbap.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2jgumveea.html


<!-- 参考信息 -->