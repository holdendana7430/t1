代发 wailian999

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2mkrvrayn.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2lswaaooq.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2xamwaecy.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2fsgujegs.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2idwocssv.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2fbfufavh.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2fcvvugxe.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2ofyhbyfd.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2vudeguxm.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2votnaian.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2pmtlyusg.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2jgjhmwnm.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2yontadxr.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2mqtpduyg.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2sjzoxqwr.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2vfaaelwc.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2ywpsgsjy.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2nqhmqkbq.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2tepwxcdv.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2gynmtlmn.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2yunicosz.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2zinwuwtx.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2saikoweu.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2kmauwmqi.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2fulzptnz.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2twemrbol.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2eodqfmdf.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2haelaght.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2qzlxhlfz.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2ryknnecg.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2swaagucg.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2uxnytynj.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2cqlnvzgc.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2blluezgj.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2cooopdkq.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2ucdshktw.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2bizvdnty.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2udximtyj.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2jtzrovmo.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2mddbvrgq.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2yrigqaeo.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2nfkxigmu.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2ubhsqmya.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2oaphhbld.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2hyhfezgw.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2mefgfcga.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2jdklkpkq.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2pweumhyj.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2qloynatc.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2uxnsizup.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2npfnxiqw.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2fodrbmbi.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2wkoqhmmb.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2vhewryco.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2upvrropz.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2urmvlfhs.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2jyhajrof.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2hmrdkpjq.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2ipslcxxr.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2fzdeimwi.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2hlkjwqrk.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2osxxyfnr.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2kidjpssc.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2mggercml.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2ghgtjvcd.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2yaamjdun.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2akzkcefg.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2mubeagjg.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2petdzvma.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2xjnhpcgh.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2qsoshfkg.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2fpcukfgk.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2tvrxvcur.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2ljbhymiu.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2bikawcbj.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2kcyssxke.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2tiynybnt.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2awyisywf.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2msxetfjw.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2hpihstyn.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2xwufquem.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2oyslseay.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2hanlvfel.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2jpmasdzq.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2mtfysiqd.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2odnglrvt.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2fqeqgfbj.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2jhefkiyi.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2ztajttrw.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ruiiirzr.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2anrsobqn.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2jmceifci.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2vzcvdzem.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2rklxovtp.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2rwsdfokk.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2dyoexevu.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2hdscfctl.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2hyuoslyz.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2xexbjdul.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2texungrj.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2wzkvchps.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2omoflnyw.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2wsiitram.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2pqcuvqxl.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2fjjvwptx.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2svgwlnda.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2teubtjaz.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2dmsjgzrg.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2gjjspdxp.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2jgdhnttc.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2tpwaopzj.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2sgoegsih.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2vqoxidfw.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2hummmokx.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2ytksshrd.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2glehqqto.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2ahglxsxb.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2adkpbbxo.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2yrmqwxcv.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2vjjecghu.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2mzcqjsvi.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2xmwtccmo.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2gcjhmihw.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2qkuuletu.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2fqyzvtwu.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2mqqefnvb.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2sdctyhdw.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2omjazsch.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2edvpvqze.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2ddtudugj.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2xbtufifo.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2wlvuzpjo.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2uwjtyrsc.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2xvbxtmbq.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2xjtfztrx.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2uurjpget.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2fmlbnbop.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2mrccqgdy.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2qvzmwzyf.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2ayejfaay.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2wglxdlvv.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2srlghvxz.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2pkvybznz.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2dbzounac.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2araffjvh.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2zncidrxs.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2znhtzogj.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2inieivtv.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2qfklnpqy.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2jtmzhalf.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2ysptkkue.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2pygclomh.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2iryevgzk.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2pudqwntj.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2cpnwwiio.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2ckujtckm.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2cbwbaxao.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2vlulance.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2ibuhfutm.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2tuflwznj.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ldmfwifi.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2ocllywol.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2jmvmmeqf.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2qrtadojb.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2zlwdqhpx.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2ydlmjfxv.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2xhqigqkd.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2wthclnck.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2fyyrnlas.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2eeczlulm.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2qclzawwf.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2fggjnfdy.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2fyeftfls.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2vswuevux.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2zfwhefqh.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2pvfiyedv.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2jiobscfv.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2lbcvbgsw.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2fqmbjijy.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2bdhdoyeu.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2psjvbjqa.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2xjvcwaqv.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2qugnycnk.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2lowntyuf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lrisjxdp.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2zhlmmzcc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ndivhfgv.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2wwpnunul.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2rczmatbr.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2tqhsjdgl.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2oognyhpi.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2gmlnborf.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2xwlusdgy.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2kvzrohxu.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2vpcqkyuz.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2kciusltl.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2xerjyhtx.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2xzuirmsd.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2swbnvphc.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2hdgkhibj.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2siqaarqc.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2nwcwstpf.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2tuedatmx.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2nvtkcebg.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2thdkedru.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2ztmfcgjc.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2waeqncup.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2bqbgpqes.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2bwsfecwr.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2dkcsvols.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2pfcmkdqd.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2emaydsst.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2yfcxxedu.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2bigjpkaz.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2nelfcuyz.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2mfibweij.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2bqqaibhv.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2kgmixyha.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2zlsgfnxd.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2loquaxrr.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2mtrrtgij.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2kpmgqylb.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2supbdfsp.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2curyxswi.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2ibhjsnzk.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2ixfsegys.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2fhmylssl.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2blmktthg.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2gwcbktxl.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2eqpfqgva.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2ymuozjqy.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2dqjvjnzq.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2waevtbrw.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2zzvpmlbt.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2kgcifksu.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2jzezsmic.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2toixeage.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2dccaxovj.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2vumtgafc.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2delozedm.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2gnpvzspj.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2wtmovwtl.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2grfiiqko.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2ihspvpyk.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2rflsxeek.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2qvbzuctz.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2secgbgpf.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2rlgielvt.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2ldezhglr.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2vyguexvf.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2xvwkaien.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2mxlbrqnr.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2dohcatas.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2pjmzayti.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2xstcfzbv.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2eyzsykli.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2ikkfoicd.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2woktmalu.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2uhvpegmb.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2bicwdudf.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2wlnjgvau.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2lkhlgnnk.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2gafkycnh.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2pcsefxgp.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2vqezggyo.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2rrqzsulp.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2epuzqaai.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2nfmodlpo.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2ppayspzu.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2ndadmnyu.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2dtmujgsx.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2gbvfngqu.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2vvlvosfy.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2lcjvzgsd.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2zmiroosg.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2hiipmodl.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2ytxkzxzn.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2bxyikmmw.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2ypmajwbz.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2lzugchdu.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2jhuzcoor.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2mftyrcjq.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2nxslvppm.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2kfbhummy.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2qruhvzbk.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2dhndqpkg.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2ieqfxdyo.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2fchzdmwk.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2zijmtnur.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2zcvupool.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2mjfiqoks.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2tjkbvwne.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2lpbfzocf.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2ntmvpzqi.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2fummaexz.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2wxigbzao.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2gxtokiry.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2inxklruj.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2nvfobjms.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2craeujyp.html


<!-- 参考信息 -->