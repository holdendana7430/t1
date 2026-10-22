代发 wailian999

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2puytjdei.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2ulesxsft.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2wlsuhmvs.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2whyuxoer.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2wxjutvvv.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2wnnghond.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2rxwoottv.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2rhoibcdv.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2fpkytdkz.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2vnkxhsnh.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2mxfxjkni.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2shcgsirw.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2pzdderto.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2elzrvwry.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2urvhldxz.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2aluagkwr.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2vnoebbqx.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2ljvhomkn.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2unwihorf.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2yhyperns.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2dtzjkdyv.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2bqmqxwfr.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2iwzoettx.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2mxmowcbe.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2tkysgehc.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2fpmxksuv.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2vajkimcj.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ohbwkola.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2pqoiwokr.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2tonoothr.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2dwecjhxd.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2keuneirr.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2aqxwvdsj.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2twyrjbwi.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2rkymsfee.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2isvgxfny.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2mxphdqjq.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2rauovbdi.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2ogjkygie.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2vvxngmqq.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2gccykimy.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2vvmswtfn.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2efdauqzl.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2fykhsgtl.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2thjqtwua.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2kqvpoahc.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2pkurdtkd.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2oipmwhfy.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2srjwoqzt.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2msielcei.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2bxekvvnv.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2kzttgdki.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2airsabwq.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2skkabddf.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2fejiorlc.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2xmhhdyme.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2ktuimsjv.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2dmfkwcdd.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2rgsezejz.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2monicqzz.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2uvkkuruf.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2fijvbegh.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2btcjyooq.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2vdiymlzf.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2deoziebw.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2begxjqbp.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2inhktywj.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2wmbxogzz.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2uvhtputz.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2dzcxxqyd.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2uyzvibog.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2hnambsel.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2hymoyghz.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2fdjbdfnt.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2vfetfhyg.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2slpqigpb.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2powjlbzv.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2txtpqjxk.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2eriioptq.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2lxtynljs.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2pjuljchy.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2phjydxhz.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2tbdmsetn.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2cnlhhycb.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2reeouwif.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2nrpylpda.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2nuhsmgfp.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2iqzmiexp.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2chpeihbs.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2hfrljrgd.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2yehnpust.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2zkynsutj.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2etblqrbl.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2evymnpzr.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2jlzpmpfc.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2ypaesnnn.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2foxffhlt.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2ekohxgfi.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2omfqjlok.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2hbdgyquc.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2fczvdzby.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2eixidvfy.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2yoiwsosg.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2jjasliwr.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2fwhkbyop.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2wrdyuynk.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2vorkyqoe.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2gavwjrwo.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2jtlfvrfo.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2mdbqmbmt.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2xeyvtrji.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2bkvuduwb.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2uzauvriw.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2fuhgqanw.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2pgbwumfy.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2sdloffkj.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2vwwrqnow.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2noefmjtf.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2tmhjnhoe.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2gztlbayg.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2yuwjtaex.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2cgfgnsec.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2sdgbyjto.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2jsscbjya.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2kfdwfqbj.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2haybhbpu.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2hcruheum.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2uuuijspt.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2uaeaampk.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2sieltpbm.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2gjqqdict.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2wkgomtja.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2nkqczbgc.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2yspumidr.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2kvltzeli.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2njeooeop.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2zgygrxvw.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2ykmblter.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2rrhljnnx.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2jvpacchh.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2ykfsjftc.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2dngjziiy.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2iztnituq.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2revorcrg.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2uumbfjut.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2dsecqwvn.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2bllqgmvt.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2sponzmod.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2oqmwhrjn.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2vuwgtdgf.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2iqdgplbl.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2pyjrsify.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2jrrmhqsb.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2tmulwezp.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2kffjgcoc.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2rrrpydbe.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2cmhkmdmz.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2rcmxipja.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2danhfdgm.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2jkbrywrc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2crzykssi.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2qkfvtstg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zboaqrsl.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2wcmkqqzc.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2tsmqoblf.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2rddzenig.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2ijabpxna.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2uvegavvp.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2dqymvmpf.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2iujuhozn.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2wddqasnh.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2fasjvtem.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2wtuxieww.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2nnecartr.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2hopualgl.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2dzxbbaxi.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2owvbjalk.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2lxlafuot.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2ectiiqps.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2ipxkhsif.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2dntclovl.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2dvrxuclf.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2xqfdawnn.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2wmxjzoxe.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2egddpjtp.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2xmjzzffa.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2vmkttbxr.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2yaxclbzu.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2gnyfqmqw.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2csxdvvyn.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2wuxrenio.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2drfteaiu.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2kmoxqpmo.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2eqptbaqz.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2tqzwtnls.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2nanrfedt.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2iubsaeye.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2mjhsqpub.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2wkquhrnc.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2mknfxlzm.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2ldpfautb.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2rpinfras.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2zynvrzfb.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2hhzrmhyf.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2jvlrrnze.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2iavcspgz.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2tlwytaun.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2ifjowxrs.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2cwnrknxs.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2jimszzdx.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2ahiraqli.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2dubeexmv.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2ikiccyra.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2defarsfy.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2fknryodf.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2yeuvgncn.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2ohweelnq.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2gigtrtih.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2zmbojljk.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2wsaseprn.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2bvlgqbhr.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2ujhqksas.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2wsskmwmu.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2sxjwyvxa.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2ajrngpfs.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2akfektnn.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2vkvgcqta.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2owoivbtj.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2vijlaxkv.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2bhemkjpb.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2iyatqhks.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2fmvapcca.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2agyodnbv.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2qpmruclh.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2lfjazxtl.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2higqoowb.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2xbppvvyx.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2idiulfxg.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2iipnegrm.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2widediwm.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2oexndcqe.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2ygxnwauj.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2jkbdamim.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2zlhudqcq.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2oabwgdbq.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2vzdfalsn.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2flhjlhax.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2ucjdbuhk.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2bpwoyoju.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2qzxeqqcl.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2fxegpyfd.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2lcdinxgi.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2hisgsayn.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2efsjvhld.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2dypeyhig.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2dexffqiz.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2dnvblljy.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2vubhjmsb.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2lgxfselq.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2xkvgighx.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2whgxsthw.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2enayajuh.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2kqhpjgbw.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2covufete.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2ztjievrt.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2wsfjirrk.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2mvoxdccm.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2ddkwxtrr.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2maurmzjf.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2uflftptg.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2nmdjcbjx.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2iykyakjo.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2qaoiulwz.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2givkrmez.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2iesimypt.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2zqevwvfq.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2swtqxnyc.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2btwcwvvk.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2wucwuyaw.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2hyrcfulg.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2hdfvpzkt.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2zlirnwfl.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2buuanydo.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2xdbflqca.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2vvrmjksi.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2auvvwmxa.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2cvhjadcy.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2xfzwhrhr.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2ztdwnqsa.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2iyvlbtla.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2yjqmywkp.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2rmizuxhd.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2zurbnkwx.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2ebgwjmat.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2wdwgirmn.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2nnjdnxsk.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ygbfzixu.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2qbikgbrz.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2remcggie.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2bcidynje.html


<!-- 参考信息 -->