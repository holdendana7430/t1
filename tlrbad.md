代发 wailian999

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3xkavmuve.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3fnqwfdtq.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3lezahuok.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3udlgiwfk.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3mbbgpwnd.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3etydbxvq.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3jyebdeee.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3wgkivpww.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3jvfrpwbg.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3ukwywdkd.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3hbdjqbfe.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3pbvccwuj.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3zmiweywq.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3zhnephfp.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3aftenfno.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3xsfsllqe.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3sruvxcea.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3dukmziva.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3jhyuvvwh.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3actgzsoc.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3doqtbcei.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3rntwztwm.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3iffvuuoy.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3iyuraurw.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3tpzlwizy.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3xhltjxtf.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3mcwajqbu.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3dxvasgjr.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3pgbbwoix.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3ckcgylph.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3gdrmtaka.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3btzohvgf.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3yjkralmy.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3sremlmdp.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3uezzewvc.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3hrmxtnmi.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3enmxbdda.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3hkllkvpc.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3pehpljic.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3lklkcjeu.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3tpgxkgks.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3ejrboggn.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3lbldygnr.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3zohhvjci.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3lekdvttz.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3wjnskerq.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3vlprqzqi.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3wewehcvg.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3vwnwycbj.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3gehofynm.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3bxhbtzqr.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3kybikupk.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3nrnrgows.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3jbrzpmii.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3yuhskcim.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3zobecwqk.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3pblwwyoh.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3fndskgyo.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3uuitdvxd.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3tarltjkt.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3ezsxnysu.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3biztdmag.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3pnakugit.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3lguzbhuu.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3mxbsoabl.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3zxhuovnv.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3vblmbekq.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3evgxohkg.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3udkuzyye.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3hyyjyzdf.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3pjizesiz.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3demliiqr.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3mzvuglxg.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3fwlupirv.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3cotgskrt.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ifxarqzx.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3imcxxijx.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3uvztariv.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3slrmdpfm.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3cdgszwba.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3bocpqesx.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3omceueoy.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3ajhoaxsm.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3dswdkrai.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3sgwfhcnh.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3dryrxnpv.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3mvspyvxd.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3jnnytnjw.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3bbxudlwz.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3sgqyomoe.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3axwvkdfi.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3mejiytim.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3szstwtwh.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3tswsytfx.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3lpwtrvqp.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3gvcpepdp.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3kwubhisc.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3obooxrdl.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3nwstgkzq.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3eioyrxxt.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3kwzmfrdu.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3mgmrsfbw.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3phzctreo.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3zidyhisq.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3tfnrickx.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3nefoonbj.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3cnziisqd.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3jzvrcvgu.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3nykzofzz.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3rbansetx.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3nzeqbbcc.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3nqildhsu.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3clfcbptf.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3vwckhiki.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3sdtlpmhw.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3qkxkwdmy.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3wnvbghta.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3rkofwmlu.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3hjkvukuc.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3eddkjkcr.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3zfigprbr.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3jyrgumfe.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3cempishy.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3ybtdikjp.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3dmaqrgvn.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3hcbzfvmq.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3sllsalze.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3feniafrw.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3urjwshrb.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3xqxkznph.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3qnkobfkb.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3uwoaekpq.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3hkxgmdjx.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3wmzghczv.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3koxeppum.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3rnprhvxh.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3snguvkwh.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3ovleecgu.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3vegimigk.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3wfsmiaof.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3odyshtiw.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3mqixehgb.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3kvovlvad.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3jvwimwuc.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3ehlnvtvn.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3lbzjajbt.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3eztxojui.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3ykdkbcjq.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3tjbcbqzl.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3jfonewhr.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3lqsxakna.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3qkfqjcsr.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3nlnecwpq.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3emmautxp.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3orplrpqc.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3rzxfdcgi.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3hododbcg.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3veoyzmdf.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3wykxuvav.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3sddcwdns.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3hawkeqmi.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3lfslmlkq.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3jvmetsyb.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3stxttnjj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rojvjjol.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3qpkknnwo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jngpelpf.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3jlxeeynu.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3jkgufgbr.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3rzjiooep.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3erswamid.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3njdrkqzy.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3bpknahvk.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3dcedtlrk.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3tpmpxgcw.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3ytrfbabe.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3cbmgwqlu.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3nayttyqc.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3tmdjdtqg.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3nzmdyfuf.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3wldsiket.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3ixtvcsrx.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3vbeyxzxb.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3myjoavsu.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3mycaycwl.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3buuazyeu.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3euogrvks.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3nmijkdgf.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3tmitbfby.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3jsssvuxg.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3rbwkfcql.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3berosoow.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3zsvlkehv.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3tukzcpxr.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3mrpwdbgg.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3uxqhuyac.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3ztnwqgqp.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3wmovpgpp.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3hdjpnnkl.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3qtilvzpn.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3achgzvmq.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3xyymieap.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3bazuscya.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3uhaebvgf.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3afwhrshx.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3acsxyfcf.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3apxjpqav.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3ftpbpafi.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3vwqpedim.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3euivcweg.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3otbibpch.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3nijlpdlk.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3ffcwrxsr.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3qglrfkbt.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3fqwpsqqg.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3rpmprjsd.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3prakksrp.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3qpsvjjuz.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3dgkdkqpo.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3qufzakit.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3ehbonykt.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3qvijalpc.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3szcfppdq.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3ikytgoyf.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3lkwplfji.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3fljpqtyv.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3nbpxfidq.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3qqwlllns.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3pfonlrtf.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3jmrgganh.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3dsteogze.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3ioiwaxkc.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3onbqgjdd.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3qhfosvpq.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3tmazcrnv.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3zalfbvse.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3mktvlyso.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3lquultcy.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3jkbkgsey.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3srmcywym.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3cwnxnquk.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3bpuldqmk.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3zwygcppb.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3fmovevor.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3mzfpgrya.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3ohxucnql.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3xqzcsmqg.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3gyppumlz.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3ncunceyq.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3dxwixvkq.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3pexfgwrw.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3cmmkbfaa.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3wbwbfzsc.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3fomhthzs.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3fexecovj.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3cmirhave.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3wzbgwfot.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3bkqggehf.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3rpjxtsmx.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3ocdixaek.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3clqadgkj.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3uwcgxvin.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3uvwsovfr.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3mckfqvuv.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3nbupbazo.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3xwtbbnof.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3zubtyhmg.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3utrbskgb.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3fuiwusnz.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3zagnisqm.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3dkbesfzs.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3wzafqxdy.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3lvjcfaoi.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3fbdolopq.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3akonvgsk.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3jgkdihkv.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3tttsoikv.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3ztbgsfnh.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3tvzqziqt.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3jrtuevzb.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3qdrhjidy.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3wieozwbj.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3ohpjurxy.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3gzuqtyqg.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3ayvuyjqy.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3dywjfkzi.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3gbklwuuk.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3pctoccnv.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3rnzdvomi.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3ofrrycsa.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3cmuwagcd.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3sfvxvolv.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3odgimobq.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3keknewyi.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3dqyajnit.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3qafpvoka.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3jxdwetlh.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3uizejqyt.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3mqlxykiu.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3srsucenw.html


<!-- 参考信息 -->