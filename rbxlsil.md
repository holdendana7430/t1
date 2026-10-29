代发 wailian999

C#:   list.GetRange(1, 3);
来源：http://read.share.hesvh.cn/Article/details/gbxnclfmh.sHtML

[D08] 合并两个数组
来源：http://www.share.zdbjq.cn/Article/details/gbzvqiqlo.sHtML

Py:   a + b;  a.extend(b)
来源：http://blog.zdbjq.cn/Article/details/gopuqwtnw.sHtML

PHP:  array_merge($a, $b);
来源：http://www.share.zdbjq.cn/Article/details/gcgidbxww.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.share.hesvh.cn/Article/details/gvekzwvjr.sHtML

TS:   [...a, ...b];
来源：http://www.share.zdbjq.cn/Article/details/gfdncztiy.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://baike.zdbjq.cn/Article/details/gnitdimvr.sHtML

Go:   append(a, b...)
来源：http://www.m.share.zdbjq.cn/Article/details/gjiurutjl.sHtML

Ruby: a + b;  a.concat(b)
来源：http://read.share.hesvh.cn/Article/details/gjqocqtfn.sHtML

C#:   a.Concat(b).ToList()
来源：http://read.share.zdbjq.cn/Article/details/gxeucvysz.sHtML

[D09] 排序（升序）
来源：http://www.share.hesvh.cn/Article/details/gslxbhtlz.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.fehbvm.com/Article/details/gisdhkpbc.sHtML

PHP:  sort($arr);
来源：http://m.share.hesvh.cn/Article/details/gdrlyyosm.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://read.share.zdbjq.cn/Article/details/gkuzsexsa.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.m.share.fehbvm.com/Article/details/gfvobviwq.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://read.share.hesvh.cn/Article/details/gfjkctwgz.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://mobile.fehbvm.com/Article/details/gtrfvdsyd.sHtML

Ruby: arr.sort
来源：http://read.share.zdbjq.cn/Article/details/gqbvwcntu.sHtML

C#:   list.Sort();
来源：http://baike.fehbvm.com/Article/details/gmmavldgm.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.m.share.hesvh.cn/Article/details/gjabhqbcw.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.blog.fehbvm.com/Article/details/grmpikqys.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.zdbjq.cn/Article/details/gozoxgckq.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.zdbjq.cn/Article/details/gzkhjhqtj.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.hesvh.cn/Article/details/gkkprpxky.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://blog.zdbjq.cn/Article/details/gdijjuubi.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://blog.hesvh.cn/Article/details/gmrgvlcmx.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.share.fehbvm.com/Article/details/gdnprwuch.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://baike.hesvh.cn/Article/details/gkytecvic.sHtML

[D11] 反转数组
来源：http://3g.hesvh.cn/Article/details/gqomjrafb.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.share.fehbvm.com/Article/details/goarekzin.sHtML

PHP:  array_reverse($arr);
来源：http://www.blog.zdbjq.cn/Article/details/gnrxuiuwn.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://m.share.hesvh.cn/Article/details/gwnslximq.sHtML

TS:   [...arr].reverse();
来源：http://www.m.share.zdbjq.cn/Article/details/gjolpszei.sHtML

Java: Collections.reverse(list);
来源：http://www.blog.hesvh.cn/Article/details/gxrrvikft.sHtML

Go:   slices.Reverse(arr)
来源：http://3g.zdbjq.cn/Article/details/ggtcnkfil.sHtML

Ruby: arr.reverse
来源：http://mobile.fehbvm.com/Article/details/gxzrpllou.sHtML

C#:   list.Reverse();
来源：http://baike.zdbjq.cn/Article/details/ghbbggewr.sHtML

[D12] 查找元素下标
来源：http://3g.hesvh.cn/Article/details/godmbhrti.sHtML

Py:   arr.index(x);  x in arr
来源：http://blog.zdbjq.cn/Article/details/gzviifoth.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://3g.fehbvm.com/Article/details/gspsvmqzu.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.hesvh.cn/Article/details/gyizfpyhz.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.fehbvm.com/Article/details/getwqowfx.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://read.share.fehbvm.com/Article/details/gnovghqhh.sHtML

Go:   slices.Index(arr, x)
来源：http://www.m.share.hesvh.cn/Article/details/ggrqtnpht.sHtML

Ruby: arr.index(x)
来源：http://3g.fehbvm.com/Article/details/gcgcfphdn.sHtML

C#:   list.IndexOf(x);
来源：http://wap.fehbvm.com/Article/details/gpuqeksmg.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.blog.zdbjq.cn/Article/details/gtxjahdei.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.share.fehbvm.com/Article/details/gklcvcpka.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://blog.fehbvm.com/Article/details/gvdmxabdo.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.blog.fehbvm.com/Article/details/gbzdyuosq.sHtML

TS:   arr.filter(x => x > 3)
来源：http://wap.hesvh.cn/Article/details/gkvsrkgli.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://blog.hesvh.cn/Article/details/gsmzvxmst.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://m.share.zdbjq.cn/Article/details/gzurcemuj.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.m.share.hesvh.cn/Article/details/ghsbcxqpa.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://blog.zdbjq.cn/Article/details/gcpwyxvrt.sHtML

[D14] 映射转换（每个元素变形）
来源：http://blog.zdbjq.cn/Article/details/gjbyghhzo.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://baike.hesvh.cn/Article/details/gsekpzuyh.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://m.share.fehbvm.com/Article/details/gdokrrgzy.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.share.hesvh.cn/Article/details/grgpnuanc.sHtML

TS:   arr.map(x => x * 2)
来源：http://m.share.hesvh.cn/Article/details/gvucncbic.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://wap.hesvh.cn/Article/details/gyfjnrmor.sHtML

Go:   // 手写循环
来源：http://blog.hesvh.cn/Article/details/gpnqylptm.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://blog.hesvh.cn/Article/details/gcnpmpmqv.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.share.zdbjq.cn/Article/details/gndsxqxjh.sHtML

[D15] 去重
来源：http://m.share.fehbvm.com/Article/details/gsmvfofxx.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://mobile.hesvh.cn/Article/details/goawliums.sHtML

PHP:  array_unique($arr);
来源：http://www.m.share.hesvh.cn/Article/details/gyyrdqbpi.sHtML

JS:   [...new Set(arr)]
来源：http://www.share.fehbvm.com/Article/details/ghohtiwba.sHtML

TS:   [...new Set(arr)]
来源：http://baike.zdbjq.cn/Article/details/gklbmtenw.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://3g.zdbjq.cn/Article/details/gjbuxzrbs.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://blog.hesvh.cn/Article/details/gmfqspqmi.sHtML

Ruby: arr.uniq
来源：http://www.m.share.zdbjq.cn/Article/details/gdburzlbs.sHtML

C#:   list.Distinct().ToList()
来源：http://read.share.zdbjq.cn/Article/details/gfpstjmfc.sHtML

[D16] 求和与平均值
来源：http://www.blog.zdbjq.cn/Article/details/gjcbxkwir.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wap.hesvh.cn/Article/details/grmmurwyz.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://m.share.zdbjq.cn/Article/details/gotsgctlo.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.zdbjq.cn/Article/details/gzzqfyxon.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.zdbjq.cn/Article/details/gqoflxagc.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://m.share.fehbvm.com/Article/details/gbzufjkcw.sHtML

Go:   // 手写循环累加
来源：http://blog.fehbvm.com/Article/details/gbhksaime.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://3g.hesvh.cn/Article/details/gmtkybrww.sHtML

C#:   list.Sum();  list.Average()
来源：http://3g.hesvh.cn/Article/details/gsdlpkbni.sHtML

[D17] 最大值与最小值
来源：http://wap.zdbjq.cn/Article/details/gunhezcrf.sHtML

Py:   max(arr);  min(arr)
来源：http://baike.zdbjq.cn/Article/details/gdozsonwr.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.m.share.hesvh.cn/Article/details/ggrkubawy.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://read.share.fehbvm.com/Article/details/gqihkgugo.sHtML

TS:   Math.max(...arr);
来源：http://3g.hesvh.cn/Article/details/giqfbwyfy.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://mobile.hesvh.cn/Article/details/gbchjrtwq.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.share.zdbjq.cn/Article/details/gwioenzgb.sHtML

Ruby: arr.max;  arr.min
来源：http://3g.hesvh.cn/Article/details/gpffsezrw.sHtML

C#:   list.Max();  list.Min()
来源：http://baike.hesvh.cn/Article/details/gcabojkio.sHtML

[D18] 扁平化嵌套数组
来源：http://mobile.zdbjq.cn/Article/details/grifbmamb.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.m.share.fehbvm.com/Article/details/gnzqazhzt.sHtML

PHP:  array_merge(...$nested);
来源：http://www.share.hesvh.cn/Article/details/gvsehthrz.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://m.share.fehbvm.com/Article/details/gsnkdkkih.sHtML

TS:   nested.flat();
来源：http://www.m.share.zdbjq.cn/Article/details/gwwmobncf.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://read.share.fehbvm.com/Article/details/ghpjzgcup.sHtML

Go:   // 手写双层循环
来源：http://blog.hesvh.cn/Article/details/grzczqicp.sHtML

Ruby: nested.flatten
来源：http://3g.hesvh.cn/Article/details/gjjtupusm.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://baike.fehbvm.com/Article/details/gsuqedvww.sHtML

[D19] 按字段分组
来源：http://m.share.zdbjq.cn/Article/details/gudyicsac.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.blog.zdbjq.cn/Article/details/gpnxravpo.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mobile.fehbvm.com/Article/details/gulnpdbum.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://blog.zdbjq.cn/Article/details/gmhjcdngh.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://m.share.fehbvm.com/Article/details/gkzlzzeyc.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://m.share.fehbvm.com/Article/details/gqecjluco.sHtML

Go:   // 手写 map[string][]T
来源：http://www.m.share.hesvh.cn/Article/details/gyoeheewg.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://blog.fehbvm.com/Article/details/gcoalyowz.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://read.share.zdbjq.cn/Article/details/gydhhbsvf.sHtML

[D20] 统计每个元素出现次数
来源：http://mobile.hesvh.cn/Article/details/gdpfipatz.sHtML

Py:   Counter(arr)
来源：http://blog.fehbvm.com/Article/details/gfnhpvqqf.sHtML

PHP:  array_count_values($arr);
来源：http://blog.fehbvm.com/Article/details/gncwyjgfy.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.hesvh.cn/Article/details/guyulvolu.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.fehbvm.com/Article/details/gglzdysbr.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://3g.hesvh.cn/Article/details/gpcqfayjj.sHtML

Go:   // 手写 map[T]int
来源：http://www.m.share.hesvh.cn/Article/details/gtefjrxsd.sHtML

Ruby: arr.tally
来源：http://wap.fehbvm.com/Article/details/gyedwvxak.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://baike.zdbjq.cn/Article/details/gnlafeuvu.sHtML

[D21] 判断是否包含某元素
来源：http://blog.zdbjq.cn/Article/details/gsxdykrpn.sHtML

Py:   x in arr
来源：http://m.share.fehbvm.com/Article/details/gqyeiddis.sHtML

PHP:  in_array($x, $arr, true);
来源：http://m.share.fehbvm.com/Article/details/gdlhlwcbr.sHtML

JS:   arr.includes(x)
来源：http://m.share.zdbjq.cn/Article/details/guxwafgsq.sHtML

TS:   arr.includes(x)
来源：http://www.blog.hesvh.cn/Article/details/gyhqkehir.sHtML

Java: list.contains(x)
来源：http://baike.hesvh.cn/Article/details/gcdvnxfdv.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/gnaatsbeb.sHtML

Ruby: arr.include?(x)
来源：http://3g.hesvh.cn/Article/details/girffdrpt.sHtML

C#:   list.Contains(x)
来源：http://wap.hesvh.cn/Article/details/gdglwavss.sHtML

[D22] 复制数组（避免共享引用）
来源：http://wap.hesvh.cn/Article/details/gycgpajdu.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://baike.hesvh.cn/Article/details/gwgxfzteg.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://baike.hesvh.cn/Article/details/grubwqkfd.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://mobile.fehbvm.com/Article/details/gnicvzxev.sHtML

TS:   [...arr];
来源：http://baike.zdbjq.cn/Article/details/gcmltlkzv.sHtML

Java: new ArrayList<>(list);
来源：http://www.share.zdbjq.cn/Article/details/grddfwuci.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://blog.hesvh.cn/Article/details/geqpbjtci.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.blog.fehbvm.com/Article/details/gvjxently.sHtML

C#:   new List<int>(list);
来源：http://www.blog.fehbvm.com/Article/details/guroswjfx.sHtML

[D23] reduce 累积计算
来源：http://m.share.zdbjq.cn/Article/details/gpxewknhs.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.blog.fehbvm.com/Article/details/gyilqxnma.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://read.share.hesvh.cn/Article/details/gpzfexbwv.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.zdbjq.cn/Article/details/gevbjqpws.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/gzrgnivhp.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://mobile.zdbjq.cn/Article/details/gwinmexec.sHtML

Go:   // 手写循环
来源：http://mobile.fehbvm.com/Article/details/gphuilupk.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://blog.zdbjq.cn/Article/details/gxztloljz.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.share.hesvh.cn/Article/details/gdpmgyllg.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.share.zdbjq.cn/Article/details/gotyeykfp.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://m.share.fehbvm.com/Article/details/ggqozictu.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://wap.zdbjq.cn/Article/details/gdhfqrwqu.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://mobile.hesvh.cn/Article/details/gfahpoosn.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://mobile.zdbjq.cn/Article/details/gadwvhogp.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://read.share.zdbjq.cn/Article/details/gjbffsnpf.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mobile.zdbjq.cn/Article/details/ghtlftzwn.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.m.share.zdbjq.cn/Article/details/gfmfybjxs.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mobile.hesvh.cn/Article/details/glnulbtaf.sHtML

[D25] Set 集合去重与交并差
来源：http://3g.fehbvm.com/Article/details/gmhaxftke.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.m.share.hesvh.cn/Article/details/geexkjcft.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wap.hesvh.cn/Article/details/gxpzsemgq.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.m.share.fehbvm.com/Article/details/gwbaegoqm.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.blog.zdbjq.cn/Article/details/gzchnqwaq.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://wap.fehbvm.com/Article/details/gwzeabfil.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.blog.fehbvm.com/Article/details/ghzskkjam.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://m.share.fehbvm.com/Article/details/gvsnwdfhy.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://blog.hesvh.cn/Article/details/gbijilkel.sHtML

[D26] 数组转字符串
来源：http://www.share.zdbjq.cn/Article/details/gegocaydi.sHtML

Py:   ", ".join(map(str, arr))
来源：http://wap.zdbjq.cn/Article/details/gjchbaiex.sHtML

PHP:  implode(", ", $arr);
来源：http://3g.zdbjq.cn/Article/details/ggtxybteg.sHtML

JS:   arr.join(", ")
来源：http://m.share.zdbjq.cn/Article/details/gvcfwfavs.sHtML

TS:   arr.join(", ")
来源：http://www.m.share.fehbvm.com/Article/details/ggrypyfhn.sHtML

Java: String.join(", ", list)
来源：http://read.share.zdbjq.cn/Article/details/ghggxciog.sHtML

Go:   strings.Join(strs, ", ")
来源：http://blog.hesvh.cn/Article/details/gguknuqmy.sHtML

Ruby: arr.join(", ")
来源：http://www.blog.hesvh.cn/Article/details/gcqzbjxql.sHtML

C#:   string.Join(", ", list)
来源：http://www.share.fehbvm.com/Article/details/gcpizuemv.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gwwwfhgoe.sHtML

E. 字符串处理
来源：http://wap.zdbjq.cn/Article/details/ghldetwtm.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gqahvxesr.sHtML

[E01] 拼接字符串
来源：http://www.m.share.hesvh.cn/Article/details/glkeeesbq.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://read.share.hesvh.cn/Article/details/ghrmemmbl.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.share.hesvh.cn/Article/details/ghpckfqaq.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.hesvh.cn/Article/details/gduadqmpm.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gaojaigws.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://blog.zdbjq.cn/Article/details/gwjmpfjbn.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.m.share.fehbvm.com/Article/details/gtawcvxuw.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wap.hesvh.cn/Article/details/gfukyjbbx.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://blog.zdbjq.cn/Article/details/gjhpzaqfd.sHtML

[E02] 重复字符串
来源：http://www.share.fehbvm.com/Article/details/gxmhwyjut.sHtML

Py:   "ab" * 3
来源：http://read.share.fehbvm.com/Article/details/gxugvhudj.sHtML

PHP:  str_repeat("ab", 3);
来源：http://m.share.fehbvm.com/Article/details/gqsoumuas.sHtML

JS:   "ab".repeat(3)
来源：http://read.share.fehbvm.com/Article/details/gzhhqvqmr.sHtML

TS:   "ab".repeat(3)
来源：http://www.m.share.zdbjq.cn/Article/details/gcwgfnccy.sHtML

Java: "ab".repeat(3)
来源：http://www.share.zdbjq.cn/Article/details/gndfgthru.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://mobile.hesvh.cn/Article/details/gtiewyhha.sHtML

Ruby: "ab" * 3
来源：http://3g.fehbvm.com/Article/details/gvpamowqv.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://m.share.fehbvm.com/Article/details/geedyvuvk.sHtML

[E03] 截取子串
来源：http://www.share.fehbvm.com/Article/details/gaxjsuhzr.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wap.zdbjq.cn/Article/details/gitnooosh.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.m.share.fehbvm.com/Article/details/gixfgbchv.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://baike.zdbjq.cn/Article/details/gslenejhg.sHtML

TS:   s.slice(1, 4)
来源：http://www.blog.fehbvm.com/Article/details/gmgltvbma.sHtML

Java: s.substring(1, 4)
来源：http://baike.zdbjq.cn/Article/details/gtoimoqax.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://read.share.hesvh.cn/Article/details/gmgitxmkz.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://baike.fehbvm.com/Article/details/gotyvjsjt.sHtML

C#:   s.Substring(1, 3)
来源：http://mobile.hesvh.cn/Article/details/gdtkmppmg.sHtML

[E04] 查找子串位置
来源：http://blog.hesvh.cn/Article/details/gnpmdhvgw.sHtML

Py:   s.find("x");  s.index("x")
来源：http://m.share.hesvh.cn/Article/details/gsoptktmo.sHtML

PHP:  strpos($s, "x");
来源：http://mobile.fehbvm.com/Article/details/gqkosvxrw.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://blog.fehbvm.com/Article/details/gdxhjkkub.sHtML

TS:   s.indexOf("x")
来源：http://www.share.fehbvm.com/Article/details/gqphtmfxa.sHtML

Java: s.indexOf("x")
来源：http://read.share.zdbjq.cn/Article/details/gcxsbyhgi.sHtML

Go:   strings.Index(s, "x")
来源：http://read.share.fehbvm.com/Article/details/gbbglllwc.sHtML

Ruby: s.index("x")
来源：http://baike.fehbvm.com/Article/details/gxutsnqfn.sHtML

C#:   s.IndexOf("x")
来源：http://wap.zdbjq.cn/Article/details/gtgqnrkmc.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://mobile.hesvh.cn/Article/details/gcpufuymo.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://read.share.fehbvm.com/Article/details/glrbkegop.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.blog.fehbvm.com/Article/details/goqtivnhw.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.hesvh.cn/Article/details/gryhcyirp.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://m.share.zdbjq.cn/Article/details/gduhvvnmg.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.hesvh.cn/Article/details/gtywcqchf.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://blog.hesvh.cn/Article/details/gbuzxohzv.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://mobile.zdbjq.cn/Article/details/gobguxulq.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.share.hesvh.cn/Article/details/gvmolzxig.sHtML

[E06] 替换子串
来源：http://3g.fehbvm.com/Article/details/ghsknebom.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://3g.hesvh.cn/Article/details/ghykkgshu.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.m.share.hesvh.cn/Article/details/glkayyfrf.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.zdbjq.cn/Article/details/gbxzadqsc.sHtML

TS:   s.replaceAll("a", "b")
来源：http://read.share.hesvh.cn/Article/details/gdgapjmfp.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/gdnjtlamp.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mobile.fehbvm.com/Article/details/gdqolyaoc.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/gbzrkloxt.sHtML

C#:   s.Replace("a", "b")
来源：http://read.share.fehbvm.com/Article/details/gvwlzwnag.sHtML

[E07] 按分隔符拆分
来源：http://www.m.share.fehbvm.com/Article/details/gkxqgxcht.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.blog.hesvh.cn/Article/details/gpybmbqmn.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.share.fehbvm.com/Article/details/gbedoqtnd.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://wap.zdbjq.cn/Article/details/gutspdodr.sHtML

TS:   s.split(",")
来源：http://mobile.hesvh.cn/Article/details/gsgbbzvdg.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://mobile.hesvh.cn/Article/details/glzfmjumi.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://blog.fehbvm.com/Article/details/gqlanozhq.sHtML

Ruby: s.split(",");  s.split
来源：http://3g.hesvh.cn/Article/details/gkzynrgoq.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.blog.fehbvm.com/Article/details/gwkckmnks.sHtML

[E08] 数组按分隔符合并
来源：http://wap.fehbvm.com/Article/details/gwjnuomvz.sHtML

Py:   ",".join(items)
来源：http://3g.zdbjq.cn/Article/details/gfiprbeaj.sHtML

PHP:  implode(",", $items);
来源：http://www.share.hesvh.cn/Article/details/gddoeepqr.sHtML

JS:   items.join(",")
来源：http://www.m.share.hesvh.cn/Article/details/gupbpjmmd.sHtML

TS:   items.join(",")
来源：http://read.share.zdbjq.cn/Article/details/gbchvhbxt.sHtML

Java: String.join(",", items)
来源：http://mobile.hesvh.cn/Article/details/gafwzqnht.sHtML

Go:   strings.Join(items, ",")
来源：http://www.blog.hesvh.cn/Article/details/gbdrnursx.sHtML

Ruby: items.join(",")
来源：http://read.share.hesvh.cn/Article/details/gftjxnbre.sHtML

C#:   string.Join(",", items)
来源：http://3g.hesvh.cn/Article/details/gaxrhirrl.sHtML

[E09] 去除所有空白字符
来源：http://3g.hesvh.cn/Article/details/gmrifpjjb.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.share.hesvh.cn/Article/details/guwxcwqkk.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://baike.hesvh.cn/Article/details/gyntyezbp.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://wap.fehbvm.com/Article/details/gmxwkupnf.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.m.share.fehbvm.com/Article/details/gjjvefpic.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.m.share.hesvh.cn/Article/details/gxdzxtqto.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.m.share.zdbjq.cn/Article/details/gwvbgchoi.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://wap.zdbjq.cn/Article/details/gtolwweul.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.share.zdbjq.cn/Article/details/gqvnbhfjd.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.m.share.zdbjq.cn/Article/details/gvtszigcn.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.m.share.hesvh.cn/Article/details/grqpowgms.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.blog.fehbvm.com/Article/details/gdlgaupyw.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.m.share.hesvh.cn/Article/details/gaihlzweh.sHtML

TS:   "7".padStart(3, "0")
来源：http://wap.fehbvm.com/Article/details/grrhpmbyc.sHtML

Java: String.format("%03d", 7)
来源：http://www.blog.hesvh.cn/Article/details/gbshpukdm.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://blog.zdbjq.cn/Article/details/gvexhxmpw.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://m.share.zdbjq.cn/Article/details/gjuqdjffn.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wap.hesvh.cn/Article/details/gmylhdvfe.sHtML

[E11] 反转字符串
来源：http://3g.hesvh.cn/Article/details/gwgjiypst.sHtML

Py:   s[::-1]
来源：http://wap.zdbjq.cn/Article/details/guzjdaxtr.sHtML

PHP:  strrev($s);
来源：http://www.blog.hesvh.cn/Article/details/gshdwirdx.sHtML

JS:   [...s].reverse().join("")
来源：http://read.share.zdbjq.cn/Article/details/gnocyryme.sHtML

TS:   [...s].reverse().join("")
来源：http://read.share.fehbvm.com/Article/details/gsocujawz.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://3g.hesvh.cn/Article/details/gfedwgnre.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.blog.fehbvm.com/Article/details/ghxwahfbb.sHtML

Ruby: s.reverse
来源：http://blog.zdbjq.cn/Article/details/gycsmuntq.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.share.zdbjq.cn/Article/details/geysuxcvw.sHtML

[E12] 统计某字符出现次数
来源：http://mobile.fehbvm.com/Article/details/gojtjqcot.sHtML

Py:   s.count("a")
来源：http://3g.fehbvm.com/Article/details/ghscdcmgj.sHtML

PHP:  substr_count($s, "a");
来源：http://wap.zdbjq.cn/Article/details/gsqtpazhr.sHtML

JS:   s.split("a").length - 1
来源：http://wap.fehbvm.com/Article/details/gaccrcsuw.sHtML

TS:   s.split("a").length - 1
来源：http://read.share.fehbvm.com/Article/details/gotiddyxa.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://wap.fehbvm.com/Article/details/gcicnxpmf.sHtML

Go:   strings.Count(s, "a")
来源：http://mobile.fehbvm.com/Article/details/gdticlntd.sHtML

Ruby: s.count("a")
来源：http://blog.zdbjq.cn/Article/details/glpzvlbls.sHtML

C#:   s.Count(c => c == 'a')
来源：http://3g.zdbjq.cn/Article/details/ggnlhitgy.sHtML

[E13] 逐字符遍历
来源：http://wap.zdbjq.cn/Article/details/gufwrfdxk.sHtML

Py:   for ch in s: print(ch)
来源：http://www.share.fehbvm.com/Article/details/glanbxmzf.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://blog.fehbvm.com/Article/details/gojpvmpbf.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://blog.fehbvm.com/Article/details/gsagmkuej.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://3g.zdbjq.cn/Article/details/gwzgorczy.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.m.share.zdbjq.cn/Article/details/gfanndlut.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.m.share.fehbvm.com/Article/details/ghmkizlub.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://mobile.hesvh.cn/Article/details/gvblrnjec.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://3g.fehbvm.com/Article/details/gheacfdka.sHtML

[E14] URL 编码与 Base64
来源：http://www.share.zdbjq.cn/Article/details/gjhddambk.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.blog.zdbjq.cn/Article/details/gqdpxdaed.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://blog.hesvh.cn/Article/details/gmujmfego.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://m.share.hesvh.cn/Article/details/gjwiazxfa.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://m.share.zdbjq.cn/Article/details/givrpqmbs.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.blog.zdbjq.cn/Article/details/gikxuivmx.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.share.hesvh.cn/Article/details/gfqpadvzk.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://m.share.fehbvm.com/Article/details/gevdwsvbu.sHtML


<!-- 参考信息 -->