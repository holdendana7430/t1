代发 wailian999

JS:   [...a, ...b];  a.concat(b);
来源：http://m.share.hesvh.cn/Article/details/gnljxuwjt.sHtML

TS:   [...a, ...b];
来源：http://www.share.zdbjq.cn/Article/details/gnuacvybc.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://3g.hesvh.cn/Article/details/glehaazqo.sHtML

Go:   append(a, b...)
来源：http://www.blog.fehbvm.com/Article/details/gjkezgqco.sHtML

Ruby: a + b;  a.concat(b)
来源：http://baike.zdbjq.cn/Article/details/gtafnmnep.sHtML

C#:   a.Concat(b).ToList()
来源：http://wap.zdbjq.cn/Article/details/gsbxwznpg.sHtML

[D09] 排序（升序）
来源：http://www.share.fehbvm.com/Article/details/gfyprzjzn.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.hesvh.cn/Article/details/gevepwwkz.sHtML

PHP:  sort($arr);
来源：http://www.m.share.hesvh.cn/Article/details/gsogcdhzn.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://mobile.hesvh.cn/Article/details/gloljoiqe.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://wap.zdbjq.cn/Article/details/ghwsgvnsj.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://read.share.hesvh.cn/Article/details/goywcxegi.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://wap.zdbjq.cn/Article/details/guvwhyuwr.sHtML

Ruby: arr.sort
来源：http://mobile.zdbjq.cn/Article/details/gopnshlyv.sHtML

C#:   list.Sort();
来源：http://wap.zdbjq.cn/Article/details/gpwbsgmwp.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://baike.fehbvm.com/Article/details/glokfcdks.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://3g.fehbvm.com/Article/details/gfdbgikrg.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.zdbjq.cn/Article/details/gptcbipsn.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.hesvh.cn/Article/details/gemrsvwjd.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.fehbvm.com/Article/details/gqtolginh.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://baike.zdbjq.cn/Article/details/gkasrkxib.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://read.share.zdbjq.cn/Article/details/gzqdjqheu.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://3g.fehbvm.com/Article/details/gidmxoouc.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://3g.hesvh.cn/Article/details/gqialifxu.sHtML

[D11] 反转数组
来源：http://wap.hesvh.cn/Article/details/gqbzofytn.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.m.share.zdbjq.cn/Article/details/gotritlau.sHtML

PHP:  array_reverse($arr);
来源：http://m.share.zdbjq.cn/Article/details/gkirkhjqf.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mobile.zdbjq.cn/Article/details/gaxlltgcs.sHtML

TS:   [...arr].reverse();
来源：http://baike.fehbvm.com/Article/details/grcwzuhks.sHtML

Java: Collections.reverse(list);
来源：http://www.share.hesvh.cn/Article/details/gndqrpwbx.sHtML

Go:   slices.Reverse(arr)
来源：http://m.share.zdbjq.cn/Article/details/gpefcduhc.sHtML

Ruby: arr.reverse
来源：http://www.blog.hesvh.cn/Article/details/gcuezcdfb.sHtML

C#:   list.Reverse();
来源：http://m.share.hesvh.cn/Article/details/gcsnvqhig.sHtML

[D12] 查找元素下标
来源：http://baike.fehbvm.com/Article/details/gvzeitbsx.sHtML

Py:   arr.index(x);  x in arr
来源：http://baike.hesvh.cn/Article/details/gdmzgrqwm.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.m.share.zdbjq.cn/Article/details/giprfgaev.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.hesvh.cn/Article/details/gahmamwox.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.zdbjq.cn/Article/details/ggnqtrwvt.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://m.share.hesvh.cn/Article/details/gxubisqet.sHtML

Go:   slices.Index(arr, x)
来源：http://www.m.share.hesvh.cn/Article/details/gasnlecnz.sHtML

Ruby: arr.index(x)
来源：http://wap.hesvh.cn/Article/details/gvokzpqdd.sHtML

C#:   list.IndexOf(x);
来源：http://mobile.hesvh.cn/Article/details/ghzrqctqf.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.blog.zdbjq.cn/Article/details/gwokxfbdb.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.blog.fehbvm.com/Article/details/grpsayluu.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.share.hesvh.cn/Article/details/gdlkviagj.sHtML

JS:   arr.filter(x => x > 3)
来源：http://baike.hesvh.cn/Article/details/gpjtrsiae.sHtML

TS:   arr.filter(x => x > 3)
来源：http://read.share.fehbvm.com/Article/details/gjokqjjqs.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mobile.hesvh.cn/Article/details/gsebqisyc.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mobile.fehbvm.com/Article/details/gmgtlvyfq.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://mobile.hesvh.cn/Article/details/gvndhkuld.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.m.share.hesvh.cn/Article/details/gptgmtlis.sHtML

[D14] 映射转换（每个元素变形）
来源：http://wap.zdbjq.cn/Article/details/gdcpjwmfa.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://m.share.zdbjq.cn/Article/details/glppuozwf.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mobile.zdbjq.cn/Article/details/gjrjvscfk.sHtML

JS:   arr.map(x => x * 2)
来源：http://baike.hesvh.cn/Article/details/gncifqevz.sHtML

TS:   arr.map(x => x * 2)
来源：http://m.share.zdbjq.cn/Article/details/gpvqdmsge.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://blog.zdbjq.cn/Article/details/gaqyfykzg.sHtML

Go:   // 手写循环
来源：http://blog.zdbjq.cn/Article/details/grxvlpnva.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://wap.zdbjq.cn/Article/details/gjajanfeg.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://m.share.fehbvm.com/Article/details/gzmggyizk.sHtML

[D15] 去重
来源：http://wap.hesvh.cn/Article/details/gxelvptes.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://baike.fehbvm.com/Article/details/gjvvizmef.sHtML

PHP:  array_unique($arr);
来源：http://wap.fehbvm.com/Article/details/gkbkgxrtc.sHtML

JS:   [...new Set(arr)]
来源：http://read.share.zdbjq.cn/Article/details/gfcnstbdm.sHtML

TS:   [...new Set(arr)]
来源：http://www.m.share.hesvh.cn/Article/details/ggkdkkojr.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://m.share.zdbjq.cn/Article/details/gcknhkxvk.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.share.zdbjq.cn/Article/details/ghxxoeggv.sHtML

Ruby: arr.uniq
来源：http://baike.hesvh.cn/Article/details/gnolsiqyq.sHtML

C#:   list.Distinct().ToList()
来源：http://www.blog.fehbvm.com/Article/details/gnxmqydoc.sHtML

[D16] 求和与平均值
来源：http://wap.fehbvm.com/Article/details/ghkpkpouz.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://m.share.zdbjq.cn/Article/details/ggiqwextk.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://blog.fehbvm.com/Article/details/ggquukans.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.zdbjq.cn/Article/details/gysubhurl.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.hesvh.cn/Article/details/gqwegqvjy.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.m.share.hesvh.cn/Article/details/guxvjypwk.sHtML

Go:   // 手写循环累加
来源：http://blog.fehbvm.com/Article/details/gksnxssvc.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://m.share.hesvh.cn/Article/details/gzbsggwrt.sHtML

C#:   list.Sum();  list.Average()
来源：http://m.share.hesvh.cn/Article/details/ghdqqtklq.sHtML

[D17] 最大值与最小值
来源：http://blog.fehbvm.com/Article/details/gmancbcdt.sHtML

Py:   max(arr);  min(arr)
来源：http://mobile.fehbvm.com/Article/details/gkhsijcdw.sHtML

PHP:  max($arr);  min($arr);
来源：http://read.share.hesvh.cn/Article/details/gkbheyxoe.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://read.share.zdbjq.cn/Article/details/glwckiqif.sHtML

TS:   Math.max(...arr);
来源：http://baike.hesvh.cn/Article/details/gpjdtwwxr.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.blog.hesvh.cn/Article/details/gjfddpblf.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.share.zdbjq.cn/Article/details/gjugbysif.sHtML

Ruby: arr.max;  arr.min
来源：http://baike.fehbvm.com/Article/details/gzzahxefq.sHtML

C#:   list.Max();  list.Min()
来源：http://wap.hesvh.cn/Article/details/gfblzajqo.sHtML

[D18] 扁平化嵌套数组
来源：http://mobile.hesvh.cn/Article/details/gtwhhngty.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wap.hesvh.cn/Article/details/gnnenrhxr.sHtML

PHP:  array_merge(...$nested);
来源：http://wap.zdbjq.cn/Article/details/gadpvpxrn.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://blog.hesvh.cn/Article/details/gitrbeuif.sHtML

TS:   nested.flat();
来源：http://www.blog.hesvh.cn/Article/details/gpgvkzctt.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.m.share.zdbjq.cn/Article/details/gktfkpkmx.sHtML

Go:   // 手写双层循环
来源：http://wap.hesvh.cn/Article/details/ggndzpilr.sHtML

Ruby: nested.flatten
来源：http://mobile.zdbjq.cn/Article/details/gikuisuqa.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://baike.hesvh.cn/Article/details/gpuvddall.sHtML

[D19] 按字段分组
来源：http://wap.fehbvm.com/Article/details/gqxudrszj.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://3g.hesvh.cn/Article/details/gjdhajzvv.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://baike.zdbjq.cn/Article/details/gcnfholgv.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.m.share.fehbvm.com/Article/details/gtdbhingf.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://wap.hesvh.cn/Article/details/gtvexzjfs.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://blog.zdbjq.cn/Article/details/gbkspfkls.sHtML

Go:   // 手写 map[string][]T
来源：http://wap.hesvh.cn/Article/details/gowdgktoh.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.blog.fehbvm.com/Article/details/geayqlvol.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://m.share.hesvh.cn/Article/details/gazffuhpv.sHtML

[D20] 统计每个元素出现次数
来源：http://mobile.hesvh.cn/Article/details/gjojguwhz.sHtML

Py:   Counter(arr)
来源：http://3g.zdbjq.cn/Article/details/gbmakzvpz.sHtML

PHP:  array_count_values($arr);
来源：http://baike.hesvh.cn/Article/details/gkuzhxmup.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.fehbvm.com/Article/details/gioyowtsc.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.zdbjq.cn/Article/details/gfpqnszeh.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://m.share.hesvh.cn/Article/details/gqulskvpx.sHtML

Go:   // 手写 map[T]int
来源：http://3g.hesvh.cn/Article/details/gzzqhiudj.sHtML

Ruby: arr.tally
来源：http://www.m.share.fehbvm.com/Article/details/ghxobqcde.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://m.share.zdbjq.cn/Article/details/gcnuhveqc.sHtML

[D21] 判断是否包含某元素
来源：http://read.share.fehbvm.com/Article/details/gptrruorj.sHtML

Py:   x in arr
来源：http://www.share.hesvh.cn/Article/details/gmgalhgxv.sHtML

PHP:  in_array($x, $arr, true);
来源：http://mobile.zdbjq.cn/Article/details/gwpjsyxgt.sHtML

JS:   arr.includes(x)
来源：http://blog.zdbjq.cn/Article/details/gxsufksyn.sHtML

TS:   arr.includes(x)
来源：http://www.blog.zdbjq.cn/Article/details/geexgpppe.sHtML

Java: list.contains(x)
来源：http://m.share.zdbjq.cn/Article/details/gpshbfiem.sHtML

Go:   slices.Contains(arr, x)
来源：http://read.share.fehbvm.com/Article/details/gymidvdhk.sHtML

Ruby: arr.include?(x)
来源：http://www.blog.hesvh.cn/Article/details/gmcgobwto.sHtML

C#:   list.Contains(x)
来源：http://www.share.zdbjq.cn/Article/details/gslxrqygz.sHtML

[D22] 复制数组（避免共享引用）
来源：http://wap.fehbvm.com/Article/details/gwyjijcpk.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://3g.fehbvm.com/Article/details/gqweuvntz.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://baike.fehbvm.com/Article/details/grrxgrnfj.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wap.hesvh.cn/Article/details/gswinhgzx.sHtML

TS:   [...arr];
来源：http://mobile.fehbvm.com/Article/details/glnhzpinb.sHtML

Java: new ArrayList<>(list);
来源：http://www.share.fehbvm.com/Article/details/gnojxalxy.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.share.fehbvm.com/Article/details/gnrvmmgsg.sHtML

Ruby: arr.dup;  arr.clone
来源：http://read.share.hesvh.cn/Article/details/ghorwtigw.sHtML

C#:   new List<int>(list);
来源：http://wap.zdbjq.cn/Article/details/gowzsbixr.sHtML

[D23] reduce 累积计算
来源：http://www.share.zdbjq.cn/Article/details/gtosobxoc.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://read.share.zdbjq.cn/Article/details/gjwgewxug.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wap.fehbvm.com/Article/details/gvdyrmloy.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.fehbvm.com/Article/details/ghwenvgik.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.fehbvm.com/Article/details/gtnotwvea.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://mobile.fehbvm.com/Article/details/gtatoadsh.sHtML

Go:   // 手写循环
来源：http://www.m.share.fehbvm.com/Article/details/gzxrbeake.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://3g.fehbvm.com/Article/details/gxrrfyvvd.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://3g.fehbvm.com/Article/details/glscobnqy.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.m.share.zdbjq.cn/Article/details/gooekftcz.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wap.zdbjq.cn/Article/details/gaynpiqkf.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://m.share.hesvh.cn/Article/details/gqlkgzvpj.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://baike.fehbvm.com/Article/details/guhhafaad.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/gieexfjro.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://baike.zdbjq.cn/Article/details/gwoinphal.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.blog.fehbvm.com/Article/details/gpjueueqr.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.share.zdbjq.cn/Article/details/gabutcetm.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://m.share.zdbjq.cn/Article/details/grykllvvx.sHtML

[D25] Set 集合去重与交并差
来源：http://wap.zdbjq.cn/Article/details/gboapgiqt.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.blog.fehbvm.com/Article/details/gswilgpiq.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mobile.zdbjq.cn/Article/details/gfimkkvni.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://baike.hesvh.cn/Article/details/gkckfwykz.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mobile.zdbjq.cn/Article/details/gkhjzohgv.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.blog.zdbjq.cn/Article/details/gqvgvmksv.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.share.zdbjq.cn/Article/details/gtonqswhj.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://3g.zdbjq.cn/Article/details/gchnanpxm.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mobile.zdbjq.cn/Article/details/gvtbcpbhw.sHtML

[D26] 数组转字符串
来源：http://m.share.zdbjq.cn/Article/details/gpemcxaac.sHtML

Py:   ", ".join(map(str, arr))
来源：http://mobile.zdbjq.cn/Article/details/gpzkjtrji.sHtML

PHP:  implode(", ", $arr);
来源：http://www.m.share.fehbvm.com/Article/details/gonldhrfq.sHtML

JS:   arr.join(", ")
来源：http://blog.zdbjq.cn/Article/details/gllfzfqzm.sHtML

TS:   arr.join(", ")
来源：http://www.blog.zdbjq.cn/Article/details/gnczcnzme.sHtML

Java: String.join(", ", list)
来源：http://wap.fehbvm.com/Article/details/gdncakfcj.sHtML

Go:   strings.Join(strs, ", ")
来源：http://3g.zdbjq.cn/Article/details/gitzjtruf.sHtML

Ruby: arr.join(", ")
来源：http://m.share.fehbvm.com/Article/details/gllgzykxl.sHtML

C#:   string.Join(", ", list)
来源：http://www.m.share.hesvh.cn/Article/details/gxgxpvxmg.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gmxtrtyjk.sHtML

E. 字符串处理
来源：http://baike.hesvh.cn/Article/details/gwxkwdorf.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gfwnigdlj.sHtML

[E01] 拼接字符串
来源：http://www.m.share.hesvh.cn/Article/details/gmtofykjl.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.share.fehbvm.com/Article/details/gcfsgqkgj.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.share.hesvh.cn/Article/details/gardavsza.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.fehbvm.com/Article/details/gcnrpvgbb.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gdhcztjnn.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://wap.zdbjq.cn/Article/details/gdvfevtdt.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://3g.zdbjq.cn/Article/details/gmyzqvyhe.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wap.hesvh.cn/Article/details/gwvhfqpdr.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://blog.fehbvm.com/Article/details/gbyfjdsib.sHtML

[E02] 重复字符串
来源：http://www.share.hesvh.cn/Article/details/gtrjurewz.sHtML

Py:   "ab" * 3
来源：http://www.m.share.hesvh.cn/Article/details/gojnfsrwb.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.m.share.hesvh.cn/Article/details/gdvznecaf.sHtML

JS:   "ab".repeat(3)
来源：http://www.m.share.hesvh.cn/Article/details/gnrlamhgs.sHtML

TS:   "ab".repeat(3)
来源：http://www.m.share.zdbjq.cn/Article/details/gfgkanwzd.sHtML

Java: "ab".repeat(3)
来源：http://blog.hesvh.cn/Article/details/gbkliykfh.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://wap.zdbjq.cn/Article/details/glusutzqz.sHtML

Ruby: "ab" * 3
来源：http://mobile.zdbjq.cn/Article/details/gtgzmrnhy.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://m.share.zdbjq.cn/Article/details/gomuunflr.sHtML

[E03] 截取子串
来源：http://read.share.hesvh.cn/Article/details/gppsuyjav.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.share.zdbjq.cn/Article/details/grtoqwfpl.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.blog.zdbjq.cn/Article/details/ghupevkmq.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.m.share.zdbjq.cn/Article/details/gnuqddaxz.sHtML

TS:   s.slice(1, 4)
来源：http://www.share.hesvh.cn/Article/details/gptyaffqr.sHtML

Java: s.substring(1, 4)
来源：http://baike.zdbjq.cn/Article/details/gzoyblmki.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://mobile.fehbvm.com/Article/details/ggoakrbih.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://mobile.hesvh.cn/Article/details/gecmohyuk.sHtML

C#:   s.Substring(1, 3)
来源：http://www.share.zdbjq.cn/Article/details/gqxiwqlmv.sHtML

[E04] 查找子串位置
来源：http://m.share.zdbjq.cn/Article/details/geitmcajf.sHtML

Py:   s.find("x");  s.index("x")
来源：http://blog.hesvh.cn/Article/details/gvaocumvt.sHtML

PHP:  strpos($s, "x");
来源：http://mobile.zdbjq.cn/Article/details/gotitqdle.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.blog.fehbvm.com/Article/details/ghzaiseen.sHtML

TS:   s.indexOf("x")
来源：http://3g.fehbvm.com/Article/details/gigclytbf.sHtML

Java: s.indexOf("x")
来源：http://www.blog.fehbvm.com/Article/details/gifwoxjhf.sHtML

Go:   strings.Index(s, "x")
来源：http://wap.zdbjq.cn/Article/details/gjfrgkhxr.sHtML

Ruby: s.index("x")
来源：http://m.share.fehbvm.com/Article/details/ggsaakhje.sHtML

C#:   s.IndexOf("x")
来源：http://baike.hesvh.cn/Article/details/gctaqpihz.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.blog.hesvh.cn/Article/details/guhizxujv.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://3g.fehbvm.com/Article/details/gyaezvxen.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://3g.zdbjq.cn/Article/details/giafrqbve.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.zdbjq.cn/Article/details/grxryfkto.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.m.share.fehbvm.com/Article/details/gdkqolcbz.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.hesvh.cn/Article/details/guihcnflk.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://blog.zdbjq.cn/Article/details/gqyydiygo.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://3g.zdbjq.cn/Article/details/gdlcmlmqm.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://3g.zdbjq.cn/Article/details/guqjsmnsa.sHtML

[E06] 替换子串
来源：http://mobile.zdbjq.cn/Article/details/gnsqiczry.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://baike.zdbjq.cn/Article/details/gmqrhglqt.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://m.share.fehbvm.com/Article/details/gkpjfjzay.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.hesvh.cn/Article/details/gyxztvacn.sHtML

TS:   s.replaceAll("a", "b")
来源：http://mobile.hesvh.cn/Article/details/graveiomn.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.fehbvm.com/Article/details/gltrhfvit.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.m.share.fehbvm.com/Article/details/gapqzxjwl.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://read.share.fehbvm.com/Article/details/gkfaacwbp.sHtML

C#:   s.Replace("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/giusnlnhw.sHtML

[E07] 按分隔符拆分
来源：http://3g.fehbvm.com/Article/details/gdoegxbdh.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://m.share.hesvh.cn/Article/details/gehreuxzq.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://blog.hesvh.cn/Article/details/gcafjpwmr.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://blog.fehbvm.com/Article/details/gfqikpyxf.sHtML

TS:   s.split(",")
来源：http://www.blog.zdbjq.cn/Article/details/gkxzgmiyb.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://wap.fehbvm.com/Article/details/gffgtxvli.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://baike.hesvh.cn/Article/details/ggnmpjxqg.sHtML

Ruby: s.split(",");  s.split
来源：http://mobile.zdbjq.cn/Article/details/glqrwvlna.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://m.share.zdbjq.cn/Article/details/gqcozgflz.sHtML

[E08] 数组按分隔符合并
来源：http://3g.zdbjq.cn/Article/details/gyjwwvtcn.sHtML

Py:   ",".join(items)
来源：http://read.share.hesvh.cn/Article/details/gmjnlaqob.sHtML

PHP:  implode(",", $items);
来源：http://wap.hesvh.cn/Article/details/glmigiqbv.sHtML

JS:   items.join(",")
来源：http://baike.fehbvm.com/Article/details/gwflhyfdc.sHtML

TS:   items.join(",")
来源：http://3g.hesvh.cn/Article/details/gbyxvkylp.sHtML

Java: String.join(",", items)
来源：http://baike.zdbjq.cn/Article/details/gypwdbips.sHtML

Go:   strings.Join(items, ",")
来源：http://wap.fehbvm.com/Article/details/geftgottp.sHtML

Ruby: items.join(",")
来源：http://3g.zdbjq.cn/Article/details/ghwqicvfh.sHtML

C#:   string.Join(",", items)
来源：http://www.m.share.hesvh.cn/Article/details/gazpgjnlp.sHtML

[E09] 去除所有空白字符
来源：http://3g.hesvh.cn/Article/details/gnvasmipe.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://m.share.zdbjq.cn/Article/details/gyaxfnfch.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://baike.hesvh.cn/Article/details/grzwnaych.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.m.share.zdbjq.cn/Article/details/gnrgyxsos.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.blog.fehbvm.com/Article/details/gpeeisuon.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://3g.hesvh.cn/Article/details/glrdvrlnn.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.m.share.hesvh.cn/Article/details/gypmxrusp.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://3g.zdbjq.cn/Article/details/grtereihi.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://m.share.hesvh.cn/Article/details/gnpbwobpw.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.share.zdbjq.cn/Article/details/gstytnayn.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://3g.zdbjq.cn/Article/details/ghrycnmem.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mobile.zdbjq.cn/Article/details/gsdallzsi.sHtML

JS:   "7".padStart(3, "0")
来源：http://blog.zdbjq.cn/Article/details/gysryaeyu.sHtML

TS:   "7".padStart(3, "0")
来源：http://blog.hesvh.cn/Article/details/gtsfnnuer.sHtML

Java: String.format("%03d", 7)
来源：http://www.m.share.zdbjq.cn/Article/details/gfqukbudb.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.blog.hesvh.cn/Article/details/gpmhchrft.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.m.share.fehbvm.com/Article/details/gpcdgiovx.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://m.share.zdbjq.cn/Article/details/gpqzrdgnp.sHtML

[E11] 反转字符串
来源：http://www.share.zdbjq.cn/Article/details/gdesvdjwk.sHtML

Py:   s[::-1]
来源：http://www.share.hesvh.cn/Article/details/ggyrdekql.sHtML

PHP:  strrev($s);
来源：http://read.share.fehbvm.com/Article/details/gpqdakbnd.sHtML

JS:   [...s].reverse().join("")
来源：http://baike.zdbjq.cn/Article/details/guswawdop.sHtML

TS:   [...s].reverse().join("")
来源：http://baike.hesvh.cn/Article/details/gqyrbkgnx.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://mobile.fehbvm.com/Article/details/gpynzimun.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://blog.hesvh.cn/Article/details/gbkaiklhy.sHtML

Ruby: s.reverse
来源：http://www.m.share.hesvh.cn/Article/details/gsrnxusor.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.blog.fehbvm.com/Article/details/ghimwpkop.sHtML

[E12] 统计某字符出现次数
来源：http://www.blog.fehbvm.com/Article/details/gcfuetdua.sHtML

Py:   s.count("a")
来源：http://baike.hesvh.cn/Article/details/gwiahlyqy.sHtML

PHP:  substr_count($s, "a");
来源：http://blog.fehbvm.com/Article/details/gdypcgmuz.sHtML

JS:   s.split("a").length - 1
来源：http://baike.hesvh.cn/Article/details/gyysezqdn.sHtML

TS:   s.split("a").length - 1
来源：http://m.share.fehbvm.com/Article/details/gotsgjisd.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.blog.hesvh.cn/Article/details/gjoioozvs.sHtML

Go:   strings.Count(s, "a")
来源：http://www.m.share.fehbvm.com/Article/details/gilzvnpny.sHtML

Ruby: s.count("a")
来源：http://baike.fehbvm.com/Article/details/gaskfmlqm.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.m.share.hesvh.cn/Article/details/gkutecdqe.sHtML

[E13] 逐字符遍历
来源：http://www.share.fehbvm.com/Article/details/gmkpkbopu.sHtML

Py:   for ch in s: print(ch)
来源：http://baike.zdbjq.cn/Article/details/gwxgtggfw.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://3g.hesvh.cn/Article/details/gbajkysiq.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://baike.zdbjq.cn/Article/details/gggwlfold.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://blog.zdbjq.cn/Article/details/gvzhukuhv.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://mobile.fehbvm.com/Article/details/gitmeikip.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mobile.hesvh.cn/Article/details/gnixnebjn.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://3g.fehbvm.com/Article/details/gymdfvjng.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://baike.zdbjq.cn/Article/details/gdkvjqsrn.sHtML

[E14] URL 编码与 Base64
来源：http://baike.hesvh.cn/Article/details/gwoadhjko.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://m.share.fehbvm.com/Article/details/gfyvpqomc.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://mobile.zdbjq.cn/Article/details/gkaltriif.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://read.share.hesvh.cn/Article/details/gaudqfcxy.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://m.share.zdbjq.cn/Article/details/gfxvmfloz.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://m.share.fehbvm.com/Article/details/gtqujdrtc.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.blog.hesvh.cn/Article/details/gugpmtuql.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://3g.fehbvm.com/Article/details/gvgacwtic.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://baike.hesvh.cn/Article/details/gipvhgtqd.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.blog.hesvh.cn/Article/details/gtlxidjjb.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://m.share.fehbvm.com/Article/details/gqhlzveja.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mobile.zdbjq.cn/Article/details/ghpvkdsxg.sHtML


<!-- 参考信息 -->