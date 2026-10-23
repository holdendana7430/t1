代发 wailian999

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3jxrqebgt.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3pslhgtmw.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3ojuggqyn.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3vfddisap.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3uhhsgwgr.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3mkqyrmkr.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3jebymrqw.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3ohxbqjwf.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3kbgjueui.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3dwhqkmrv.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3aexenhoa.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3abxnstsr.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3vtcclfyo.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3khesxrui.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3peqgeuch.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3kqdptfaz.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3cwhxwzgx.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3brtuqmsi.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3xxzqpivh.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3tgezqenn.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3tlyuggmd.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3ulojruux.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3kmubelzw.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3ghhqqzwq.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3diyfroka.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3rsaxvhkw.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3cxxnrppp.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3ovnneokf.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3nsgdltbk.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3hhebjwbz.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3vhyhsiws.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3fqjitgau.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3kzmqnzaf.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3wyxqspws.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3gaycbpdy.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3mradqrty.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3giythhky.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3fjbjlpuz.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3nenczacl.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3tclufsfz.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3nqkkcasc.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3lormwbft.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3wwdtliep.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3ujoxdumo.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3hdgcgkza.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3synfxlve.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3lxqbwjqb.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3mahnjqnv.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3dbjsrrzn.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3kbjvjngn.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3zfzazthr.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3ynxujkef.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3mhbflcuz.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3gqavgayh.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3wwylkovb.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3cvovrkxl.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3vbzhnotw.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3syxxmvjc.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3qassewpc.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3mfklbdld.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3kynrzonp.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3rdsqherv.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3msxvleao.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3ilvhnfab.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3kqrwfhwz.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3brxatdjo.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3xorujpuz.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3nkobdjxo.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3fvnhloot.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3ouwyubpa.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3kieogszh.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3lxxoshde.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ynokraat.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3keegdaxt.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3nwdlnwgd.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3kmqjsmxo.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3lwbuweru.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3allqhoae.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3uxzfeinc.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3rrsmkocc.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3tfumkvtp.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3gqeyksvl.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3afgennzm.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3tyubakob.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3pohfxxid.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3sikevtua.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3ubwtxozb.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3ibyqaaed.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3lxnckwya.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3ykviphsj.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3dovocgbf.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3gztyxqfe.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3teigwkhg.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3okxvbhjx.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3qjavxbpo.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3ipkajvhb.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3wiegscqd.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3krnkgpft.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3dzgpdfgi.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3ivbvcxoc.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3swsguper.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3hxdvktim.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3oagpfgnw.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3sdfgtjyp.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3kibzznvq.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3dgrqifpf.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3icyuwaom.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3joomvmst.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3okrenxvn.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3ptcmnzcr.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3ssuysobu.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3dfrwusnb.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3uztxdaal.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3rdamhcyq.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3dzroqjop.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3afmaioot.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3rvehzyaz.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3ridzehaq.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3pgfcirgx.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3thgoshyt.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3jkthmycl.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3lppxuzzc.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3qtyooqbg.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3cpalvqqf.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3pexgrtpu.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3lawadvul.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3tfndbflu.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3lrnygisn.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3afjbanme.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3memdyknq.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3dyvtiemq.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3apautcqh.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3cxduibjx.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3lvghuqzr.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3scwmxfpp.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3pesqgkam.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3fsvxtzek.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3yhjcaehp.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3mrzyhipx.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3mnzmrmbn.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3ognphivb.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3dqzakppl.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3xvqoikhp.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3wewaagmf.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3cgpodopu.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3cbkaykgy.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3bcdfvrin.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3qqxhmsix.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3panygrbk.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3oorfnhjx.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3zzzsqtkk.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3gbigpzem.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3nlxlkaxd.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3zjxgfoef.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3rfceebfq.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3wpdegemr.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3igbbtpdf.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ljqiquus.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3qmyzoxrz.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3rscchgnb.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3jymiuvvm.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3qzsoyubn.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3znqcgajh.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3cvvhwpjr.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3pyawjttr.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3aetmrqsp.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3llylbpbv.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3ggsdekba.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qfkupjbs.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3beprpwpq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gnwfbrht.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ridafbko.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3gagjhykg.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3wbngzxqd.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3xkahdocq.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3rvmkwpxt.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3jqiohecw.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3pwizbvub.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3wlnxvker.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3dlxzdfaa.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3rpviqtmm.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3byksktnn.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3pimkuene.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3lwmfotrg.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3btswsmsw.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3wmxmeqjd.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3uplfaude.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3rmmckgzc.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3kqntejwm.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3vpbbkssp.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3wmpsfwhe.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3mzwxzhqp.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3erzqwwgd.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3xiqmhouu.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3behamuzx.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3htlxoujh.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3dziykrpl.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3lxeyojia.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3jpchrjnc.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3jgfyoosi.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3npluqeyd.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3gbgcsjzh.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3bzvhqthz.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3hvmrtfpx.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3nfllmign.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3snwnrxdb.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3sdilvzgq.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3kfhxcuik.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3iypxqsni.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3sasyzcrf.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3yayotree.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3dyppxqqb.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3ssegtrcr.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3mzqchxvm.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3iqrnxgbb.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3qldcvuip.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3tpfjdfek.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3qollxcly.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3arqhuhbc.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3zpdgswdv.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3ykdtikne.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3xmaakzdv.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3tgtkwmsv.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3lnqgadul.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3brrkqqud.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3otamohgs.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3ruadnkvt.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3sjpzmfkw.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3ahmrytmk.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3njjonpub.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3rklkoclw.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3glkfuczq.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3dmmztaen.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3iedklett.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3iabzwtrb.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3xslgnehw.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3hzvlcfng.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3rzcutrgs.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3qkihjkah.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3nnncfklw.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3iiykkhig.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3yywfuknd.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3sljzxinc.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3fxwawrkf.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3nncxeqvi.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3dsucjwrz.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3owmuicuv.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3ajoatzxv.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3guydrnsq.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3vvaawlqh.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3obsvmeia.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3oqhvexrz.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3xdouzcfs.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3uabpyhrn.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3zcbmvnqz.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3ebopbppq.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3vdjjbosv.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3vtpxwitu.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3kisalirf.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3zliobosi.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3bblcczbv.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3wfthrizh.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3aauhzjxe.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3ixdwemvs.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3whnqufhf.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3fbxhbxtk.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3tvkfllcg.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3vokpshsm.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3fiucnqfz.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3ldxpujwd.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3hxzbkzta.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3rwhcniza.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3zysizpfa.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3izlidvcj.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3jdswubfr.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3jrwkfkgg.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3holoqtqj.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3nwlqsksc.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3paqfylgo.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3wqsgqkme.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3lvjtflyw.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3flchspyb.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3tywhixek.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3rvoeghov.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3qzqmaoex.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3vgfcppur.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3skfucooh.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3gphrphqq.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3yjlnzhtf.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3dmupjqtk.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3xixstviw.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3imvwefrw.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3tvzwgaaq.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3qqtokgja.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3wwvlxzhc.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3vagulfon.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3jlfzlznk.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3wfyjzwaq.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3pipkcsns.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3ptvfzhmf.html


<!-- 参考信息 -->