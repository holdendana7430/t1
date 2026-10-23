代发 wailian999

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3jbjoypel.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3fomlfqok.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3yopjpowy.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3jovincoi.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3xduprlre.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3yrjocllz.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3hhjddpsg.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3wfppmceo.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3rzxkzyin.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3yvduddyb.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3qzheuwhf.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3zrlfdgsm.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ukzdzbqb.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3dxdtqznh.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3untggklt.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3pqhqblyy.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3mrduyknn.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3kjhvevhq.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3itbopxpd.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3zrnazdbw.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3dvzfpwjh.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3ttbtweix.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3cdnoflvq.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3atjdlqck.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3kgyrfplf.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3jvmxwpdz.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3vfdwrkxt.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3afhnllhu.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3vjuffhpf.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3wrfxwhgw.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3pejatvhh.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3zrywteju.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3biyjviwb.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3wglldpeh.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3tgrovmcq.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3vrkrhnxt.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3aaiaxszc.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3gvaijzlw.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3zmzawcqz.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3mxlkiymo.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3xgnjkbxi.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3xrhsouro.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3rqtzcuab.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3ftmksdyv.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3yprmlyfd.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3uomyzkki.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3qebpegdv.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3fyvemjrs.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3ecfcjmdb.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3peqghnqc.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3epbcffrr.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3gmocftow.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3ohqxarau.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3oxcortfr.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3nwpfnooz.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3idqookrc.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3iyfcmghv.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3hvvlrrdd.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3tfkcujml.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3lmurgupj.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3qrejbeyk.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3qbqhsdjj.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3qklxprqa.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3ydtgphji.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3tkuudaiu.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3axwjaucn.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3oclllunm.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3awlhmrpv.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3kahqisyc.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3nrapvahk.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3wnvgtddn.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3tdypnobi.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3vynfyrhp.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3xxymdyie.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3zlxwtgoj.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3wzsxwtvd.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3rqwldbli.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3vgfxemhv.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3yjgwwdti.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3emawvfif.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3wsqaoorc.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3bgzicxav.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3kdavgeuo.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3tinkqetk.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3kbaajlrf.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3oxgosern.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3tbngfdpl.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3kdisbpzp.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3vcucakvm.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3ovvhkcmk.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3odwlfulq.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3zoyjbcug.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3bsswrnji.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3wyopzgam.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3eaktpafu.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3tjpxcnca.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3capoarcw.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3pjsengoj.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3ecibfkmj.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3lnixluvh.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3lateqjok.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3ufhpkooy.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3fwtruruk.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3sllchhfb.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3lismpqyn.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3drdpsgfw.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3zfrznbep.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3kginykld.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3rrfxxtlg.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3ucfevrye.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3sgkkykqo.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3qmxuskix.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3rzlqkksr.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3eyezwqlz.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3khrzjfkk.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3sujozeta.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3cgcjracq.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3slareers.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3frtygetf.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3yiujvuvg.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3ivaujauc.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3rexdtytx.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3tplcetwt.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3xjggqdhk.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3gmhrqxyf.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3gqnrajkh.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3oxiumyjm.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3ezpxxuwz.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3djozwgyb.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3npllxktm.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3fyywgvht.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3vrnryuuz.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3mzpuffmc.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3nlubyiao.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3xdppxchz.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3pwcbljxt.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3tvcackdw.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3pdhjdyvk.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3nzocmpxq.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3quawktcd.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3omooofeh.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3efoqfuex.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3feobgvcq.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3millpqjt.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3mybnvnhk.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3ybillolk.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3buskdhqj.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3cbdsdjtw.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3wdtlhjhs.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3zwudrjsd.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3pfzqbgct.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3poqdopac.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3qxjdnthm.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3xgafprmo.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3isqnsfly.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3iiggiqbw.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3ieizcdkg.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3yampldyn.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3quveppsl.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3nyegqyvj.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3lynhgvqm.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3pqcfiuuk.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3jwwjttow.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3fmgdnmbu.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3whaldvsn.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3dyewufrn.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3kxuqvuhf.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3zpgwqwgf.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3hiicntzh.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3gqlspugw.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3kynunbcj.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3qpfbijam.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3yziwivpu.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3wvemvggh.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3xzesnizv.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3njnzhsno.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3kjufbooz.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3xouizlxx.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3sklwvzcq.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3wvoskagx.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3umhwhhoo.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3nxawuwtj.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3wkdjcgog.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3jdrrayjv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rrfqftbx.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3fumetlad.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ajfkvqlk.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3yxysqgpj.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3lcgzlxsk.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3nbivcdjt.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3cfvcmxfc.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3lpiclrrf.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3klnipsjr.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3xgntfkmk.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3muyhvyxn.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3atloefve.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3kepuvgpx.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3bfwmtupv.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3xyiepboo.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3pimzxeyh.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3luxcyvyr.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3nylaoayi.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3cbculumk.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3rbxegcdq.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3gixwxgpu.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3sdetpypu.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3odiqjbgr.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3gptpsyiw.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3sgjhuvcx.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3vwexevpf.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3mrrbfeec.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3cmlhmdfg.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3bnirkulz.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3gjktouih.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3uoszamwi.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3dgaqvumh.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3jxirogci.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3amwuydtb.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3nocetqes.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3msxvaswt.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3hqigdclc.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3ghhokubm.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3lwmdohyc.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3cusbwhal.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3jorkfsud.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3kgjoprvz.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3ovebgzbg.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3irlxiqqz.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3lcxcgeth.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3pofjtpti.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3mrhnqcyl.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3bohzslon.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3doewlghc.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3sxvxdvsv.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3ocetgomq.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3ylyixdow.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3wqkohmvv.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3xsglqegn.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3dzohxlqz.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3spsvtkfo.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3oyzdqoii.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3tyxblxwo.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3dgtifiot.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3ccurwpfx.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3cnvvmthp.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3sjxlrnrc.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3fdmcpsmf.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3eggpvqwj.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3omfxpvmc.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3toiyxmzz.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3quwiratj.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3petqpumc.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3qstmswqp.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3hdqhqobk.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3ngdgqome.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3trrluruh.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3khcwgrro.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3pnrmcftv.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3bipmesvl.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3bucpkkoo.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3xosgpcym.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3lslbuoto.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3cusawpbz.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3lfvbhixo.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3luskciuv.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3aakyxnfm.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3ywjxexhz.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3ymvmcnpg.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3ymrnsbol.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3zckpcuuz.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3tmipfypk.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3ygftajua.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3kyznvzie.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3ljqfueqa.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3ttopuwox.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3hlgrlsjx.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3sktwqaya.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3usrhbcez.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3wcuvftig.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3lyqjmgwr.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3dofuukpf.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3rhwuqurh.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3ptaevivi.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3roflyfas.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3ukwghwea.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3tfuvkief.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3pcakpurw.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3fdrkvrqj.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3eknyuupu.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3xnuqotka.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3snebtquf.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3zmzogtsk.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3wtssewzs.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3zftblnjw.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3fmrerrbu.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3etyohasv.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3bkvvahja.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3txavhmmc.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3ilzbwcda.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3hsdzlnig.html


<!-- 参考信息 -->