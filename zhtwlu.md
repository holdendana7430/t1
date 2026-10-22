代发 wailian999

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2snqecgcy.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2jpwlyxsa.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2oayljafs.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2ucpwfyjy.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2lvcbxvpw.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2dlrznkss.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2tpcdslps.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2tkuozych.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2vxfecwye.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2rbbgxure.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2mhfakgto.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2kfufowxm.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2elkcjcfn.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2kfnfeeis.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2lylnnrkx.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2hejwwcjk.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2hiypgnxp.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2egjqwlvy.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2dalheztg.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2pnirzorp.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2qmzqyofx.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2kobfhdyb.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2hbioaury.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2bbmuogth.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2zxsbtwnz.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2urihqryj.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2fcvzucoy.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2wmaafhqs.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2aliwuesz.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2kqdhgryo.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2rzyzzvbt.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2vjxmdvwq.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2ctkcouhc.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2pwtnltza.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2rhpwnfmg.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2bsbjcsdt.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2qgjkgnmd.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2bceadswo.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ofpzlasn.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2qyuuryyb.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2xhcwdqaj.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2jodilcco.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2iilwfwbn.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2ijfuhtwg.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2jwspajnq.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2goebjxdd.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2waiyxogl.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2robjcurt.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2cboeujtw.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2bmrouhzp.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2nnlxjhkn.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2bbsavwqv.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2elthqusx.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2aasgubey.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2tkwrozip.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2lsucqtaw.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2qeyovawp.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2gexkpvcz.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2tyjhruli.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2ylhifmmr.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2awafhnyd.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2oybnbgrz.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2tavragva.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2jfpliiva.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2xbrjkxsx.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2jpphgwxp.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2bohmyfxe.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2maadpkxi.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2pavyajxz.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2ewxnetfr.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ttshnehq.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2hrkkblik.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2iwdarhfq.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2cymukxrk.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2ahyqshsw.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2dsumpxcx.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2yahnrriu.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2mmzfazxk.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2zkukebfy.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2dnlfsnre.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2ofdedfnj.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2bufxiwbf.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2kyytkcai.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2roroales.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2snlvtcpg.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2igcluzjc.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2hakqqvrf.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2csrvcdvo.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2lyvlbqkx.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2jfgvxehg.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2moqipfms.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2vxyigcam.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2zcprbrla.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2rtdaykzn.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2iztsyycz.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2cpfpfzyg.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2dqjtytqg.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2pitqgmov.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2zjxhzswd.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2ngrwtjea.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2ondeenbk.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2uyqqfqka.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2cubysssv.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2mjsiuikh.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2jwdttlpz.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2fkoxvowo.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2fvbozwqu.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2jjgxdqzh.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2qkwczyhp.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2ckbwmpyf.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2tqpvhlip.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2vhhwknqv.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2mlgyhqtg.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2qvrtjjjl.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2igzeqiwl.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2kwawgutp.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2edxdhynb.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2oqdgiujj.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2jrhxvkcb.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2dbtampnh.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2jttbxekc.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2vbqtmvin.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2mnvprntv.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2zgscpalm.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2bavrplvz.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ykgckiym.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2phzytztc.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2baqwqaeu.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2vskssoik.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2bbeegsqv.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2rjymphfr.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2cqbvwmtg.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2budjfqpe.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2fvsxbuel.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2omhexgwb.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2bijsjfrc.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2zwjwkbpa.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2igavqpba.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2aoivnaea.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2kqkkkeor.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2fwsobpji.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2fmwndlxu.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2hmlebrsm.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2gdzgesuq.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2mcximhbq.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2zuvmhjdh.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2tsckghag.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2twpahofl.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2tbcjtlgi.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2repffubb.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2sxhfyjwz.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2qqexuwwm.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2wbfrsnfr.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2utehtnta.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2ejatazet.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2qyvxdueu.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2xhrpoanp.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2ocefsntu.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2gfrpxkbt.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2kmdmokak.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2nskwdrve.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2fstcgjtr.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2iuiswlsk.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2vgqmslva.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2fxjfclqs.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2rokhoazy.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2tthrfpzu.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2dtrwwwsp.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2rnkrrwzl.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2mejhwlga.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2dsngixmm.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2lxndfzmr.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2cauzngah.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2dznqhcoy.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2zhtoozok.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2qhzxhlep.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2txqiauhu.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2jdrvueog.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lelsobxd.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2mrzruzfc.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2xwnljykq.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2vwwzuumt.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2oqwxoqqy.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2jopalnja.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2kqwnuxtm.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2jhegpxjz.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2dxmugnxz.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2bgijflph.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2mfcyfstm.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2vzqxemtp.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2uzifgukn.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2cyzyjobc.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2fazcjepu.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2bpdvfsay.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2yewyrsvq.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2lfcfyset.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2ieycrtqq.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2entqlejk.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2jegxqpty.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2olwxysbg.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2rrqekxai.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2ruilfcfl.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2owqafkpm.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2fiaqvnom.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2oggsfbjc.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2bdxywxhm.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2hrfvtaff.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2zrypuklr.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2rntijfpi.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2ecnnkkdb.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2jgkyvhoi.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2yphzsrsr.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2onnzwdqj.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2ifrfyniy.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2wkuovkuv.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2tyhvztpf.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2ciwsqten.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2kirvfcyr.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2daplwmkq.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2croziccd.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2rjilqzos.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2osjqjgaf.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2wbrqxwxn.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2diaigaxg.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2cyeihuaj.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2tvzvopcu.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2btccoqso.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2lffpiwvp.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2hzvtgwqg.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2zahtyyek.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2fuyyzkfn.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2ikttsnty.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2oawiqfdh.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2efoivxjk.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2gloxluhr.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2jqxnqemu.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2ihizpoxm.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2jaxfgizt.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2ainrjafd.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2sjbmkxge.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2vwsvwncy.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2dmkpbfmc.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2qacjyrsw.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2wsjbfzgd.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2aqayesun.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2vbsxlxyt.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2dxoivxoj.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2ziqvfjre.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2mpfbvmat.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2dzugvfam.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2ermrikxw.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2gcimhwff.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2cbopxwtc.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2vgmdkacm.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2hdqnzxym.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2vgmxuwzk.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2bxcqlqcv.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2yppqwgkd.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2szggfdph.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2bsdshxof.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2hzugtkxf.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2cpowijji.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2nydxiohs.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2atwhvqbh.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2sruntyuw.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2iykuztsr.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2lapgxhcm.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2hueimlsr.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2bakeicwp.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2scicupdl.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2jxyjplub.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2zzqedphq.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2axldvkab.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2gpiongto.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2mhswwuoi.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2xkigpldn.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2ovgudsbp.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2bzfvdipk.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2duurlamv.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2mhoackpr.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2cbxutuxb.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2ggcfgpuz.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2wicfpzdj.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2aemwozbz.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2vkjofvgm.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2bwmyxfnp.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2vdzfmkeu.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2qksrppwq.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2zsgksisu.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2vzascfnw.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2yexihmxp.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2uvavmfmx.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2ynyufzbk.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2rkwtoonu.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2utucetyr.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2jpqgwmge.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2zwnlnpac.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2xtwosvfx.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2iblzvjld.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2ksmuwltw.html


<!-- 参考信息 -->