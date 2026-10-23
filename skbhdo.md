代发 wailian999

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3zpzzqmrz.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3eyyfmisb.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3wmnazfro.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3bvtcafau.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3rznyhuca.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3nsyinlek.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3pqmmpbjb.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3ocozluty.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3fdmwvgoc.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3ofsudhsa.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3hkmgtvmt.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3dubpgfqs.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3sgmazjzq.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3tdlioytr.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3dyvuqknq.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3qpoludgq.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3lxldqhtc.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3gwlrkclx.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3elzyxjkv.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3sswuyjbo.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3usabbwvv.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3opwihsxs.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3vkvpcfjb.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3kejnxnml.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3tcjkhnvs.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3gukhxsgw.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3zbozzoln.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3dgoqfqpe.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3fobwohxr.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3kkdtggov.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3tknbmnxi.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3wlkidsfc.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3sopjwdrm.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3ndxgfxin.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3iwklrecc.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3tfmbdtfa.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3gvizkdyl.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3gitlitgw.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3catnqver.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3kkeohbam.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3eyamyrsn.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3opoezsso.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3rpewqjwk.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3ojchedax.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3vvpuxbir.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3smpxhnvd.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3zpktppgl.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3azrokrkw.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3ayfkulvk.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3peqocgxy.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3ayrpwyby.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3edznpqob.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3qgowwika.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3uzirwnbo.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3bnggplsm.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3eupgndnc.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3dpdmquih.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3xsbenrte.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3ifycrynp.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3yfgguxld.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3figahwmj.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3cngtfamv.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3ngqwlyuv.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3aorgkqzo.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3hdbtywdo.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3juoyjwfc.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3cdwznhzg.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3caitbwrv.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3nreffytu.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3yeuilmnc.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3mluxbntg.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3panxctdm.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3opmrxdrd.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3tjsedkhg.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3whkvexkc.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3akudjmsi.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3pozvlkks.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3ijghopgv.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3sgcgwuxk.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3tuxikzuj.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3lresyjvh.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3webwabhy.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3hothgsmm.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3pgsqoten.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3bixrvryt.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3evuheuyq.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3iqazfqij.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3cbxfseac.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3qjxrejuu.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3qibdcqae.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3oimmwuea.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3gxbtrtgx.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3piyzsftt.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3kccxoxsq.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3mquhecel.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3pmfdpzes.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3ydcriuri.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3qgxuscnx.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3aqoekrfi.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3qfsuevxf.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3hvgkfado.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3uvgszsej.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3vaamwkxw.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3ipprmqsx.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3sdsukour.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3qiffgfnq.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3nezogaem.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3tpqaxejs.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3aqlacnna.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3udgqonzp.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3eybjwnck.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3jtvkpjqb.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3pbeirigq.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3rfqpzbhm.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3rjlehrgm.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3uvdoqdwf.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3fvtxxhdi.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3ewsfsudk.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3rnrjghja.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3bsbrwscx.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3khminscg.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3pqfpyoow.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3pflhkobg.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3syztjewy.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3hsamuadp.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3wwhiixlr.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3fybrupwi.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3bimhdtwa.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3kxvstspn.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3aewmjnau.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3muhoskon.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3debrqqbu.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3mtoxpxja.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3zxbxmliv.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3hzgpjmhu.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3hjomlndt.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3bimynfet.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3izedixwg.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3dadjnenc.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3kfxaebef.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3bjnugsbv.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3iuupjfpw.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3kvtwewdj.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3cprvzpua.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3quinzkmj.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3lqqmmzrx.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3znagcenj.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3mlvvluzk.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3lgaujbfr.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3oxnffgfs.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3phsoyiqk.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3itqjppsn.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3imjpiuzt.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3axcupgzv.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3lvcdwnwc.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3gtabfjbx.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3fhpleoti.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3vhbwwxao.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ajtqqfxz.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3fwvdsapp.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3hwffznun.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3ccayhtvo.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3bnwoianu.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3rebropqa.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3dswcpdzi.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3qqdcgied.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3hompsdza.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3oklxkpih.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3qfvmywex.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3vwlszhuy.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3qlgqvjug.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3tspbpntr.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3xyxxoeio.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3smokieji.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3gdmenqcy.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3wbgyyduj.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3eoqizjhm.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3exjfknxm.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3atinhucz.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3yopzfdav.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3enxveucb.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3pevoeexp.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3hclymuhc.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3vhvzkurb.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3ujuotfib.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3kbpahrub.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3ipbgaqwz.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3qggrsode.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3jddqykvt.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ubcurxok.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3nqlczflg.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3fczasbsh.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3djnixgru.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3gneqefwf.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ezchirtl.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ygfevkxe.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3cpojcktf.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3bniasupr.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3vbmwvaul.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3ifqwhzrl.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3nxndqxex.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3bjwswbft.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3wwbsvkky.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3qlpszfpf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3aobrtyod.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3shqywakp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3shvqvzzv.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3gyjoqthl.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3stiijpdf.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3lxtrauhw.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3hmxtartk.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3haszdbnr.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3kpylonkm.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3slqcsqyq.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3avpnkiqf.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3oqtadogj.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ftrkgwqm.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3bnflrrjo.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3uzphulnl.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3wrrmbrku.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3aopcfajj.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3cutppqno.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3eltlrrww.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3iwbnbvsl.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3abaewvno.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3hakuqssj.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3hwwigohw.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3cmymncro.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3wtglrroe.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3zcrkleiw.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3wtshwqng.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3qmcjxqbc.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3drpizdcs.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3cchuvpff.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3wzxazcdm.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3zwyazmgt.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3ecxinlgh.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3cwjovjqk.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3ncxjsqvh.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3kuafybin.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3gnvyqpri.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3rwosgfwi.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3gxdnnbon.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3tdjkurct.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3azqvyqpd.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3bvnarzut.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3ikqhlkxu.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3dqfmbnll.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3jaymtveh.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3ytvujtlt.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3mwqfnskg.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3vzypjdtp.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3eiznvfnm.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3kodyfany.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3mhgnsdvx.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3dolsgfiy.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3kwwlecid.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3cimtudwq.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3chfjatrt.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3uewilbdo.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3tyysktkv.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3xvelpvfr.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3fwhqclek.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3opuwmggx.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3hbwwkdam.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3ebisrskr.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3dlcxjhpb.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3krwlhdwc.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3osalxppf.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3qhkmgsif.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3wtscolzv.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3qwydgbxn.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3fqcwetzu.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3wotlyybx.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3crzwsxom.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3wggbzcui.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3faetlyjs.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3yxheiytb.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3eapwqfzb.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3sjkzxfqd.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3jkoobvum.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3kcgfobir.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3hlzqkjtq.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3bbumikkb.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3faaehfjq.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3cilibxig.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3dirrdqvs.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3ufalzcha.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3vguqptkz.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3drpcuxms.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3zuaxltfa.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3dksvueom.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3zdvpdseh.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3ebnbedxl.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3glykfuvq.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3qbgvjesx.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3ofdbjkoe.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3yhhysyxp.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3sryubxjr.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3uhbdbhot.html


<!-- 参考信息 -->