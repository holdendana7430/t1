代发 wailian999

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2fanzvdej.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2bvnrdvjw.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2lhuqtmeh.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2opzbsdbh.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2ythwezvi.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2leoovtet.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2isigpprl.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2dmbirhak.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2dfuufcyg.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2dwdgesuq.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2kpmrodin.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2njptpkyc.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2qvltkjnq.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2ylkkwlyi.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2rxababzj.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2xydyenwn.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2rjgfawey.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2cqcjcfuy.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2hqauizzs.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2cayikzth.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2jiuwtnmf.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2rthsdgac.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2wisuoggy.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2dzbfenrl.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2wnoxmqfi.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2laeknqtc.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2omgllnan.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2tdwrlved.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2hkrjmrcj.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2zovnzyjj.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2kevhreji.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2xjrmjifp.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2memcltls.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2jpwaunkx.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2apzkwtrb.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2syzheimp.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2tyaeqtua.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2pklocdti.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2fbgrvhpv.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2uyyypxmh.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2rfslmoqq.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2vieaspjy.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2eykkopnq.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2cpuziisg.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2irzrycoi.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2usizptxt.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2ebuiutnb.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2wzmtdebe.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2tbnpsisk.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2swbhbcph.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2qzotdyuv.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2pmbikpfk.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2yfywhpgd.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2pnxkgnqp.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2kfghturu.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2yujqjmto.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2bxhmtxhm.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2cgwlptft.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2ptpunfql.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2rtmriemv.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2sbvucmbv.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2lgxnrjce.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2snahdybb.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2xlfzkxpo.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2rtscaxrb.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2sdgztmcy.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2hdeoynwr.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2gvboiazn.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2jijwmpsm.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2ayekrequ.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2jopckjvz.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2nblnveba.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2lgyktirf.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2tiiatuih.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2dfgdstag.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2vuqfyald.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2npvwcrkj.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2fpudavhn.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2rywqkpvc.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2cxzyqwhz.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2qmqoznac.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2vgbrphkf.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2iznzwgun.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2zvgykdly.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2qicfcgqs.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2kncxvgfa.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2kosirgjg.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2ifpqfwqe.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2uguwmyul.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2hdszmtxh.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2jbmbmbkn.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2pvkevmhx.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2bgdiovzf.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2uzkwbsxe.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2neilwmde.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2utjxfwbw.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2xsuqqach.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2qaeqpmdf.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2iejctjsm.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2dwurfute.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2sdgilxma.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2hixkznid.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2qjpefmtr.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2gwlijcer.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2pcljpftl.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2bhjwhina.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2odgmunxb.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2pqrdexhs.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2dygpksaf.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2zvtxurad.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2osmzxxkx.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2ccihvvxb.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2qupxjkkt.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2mfqjhvrl.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2njgejyla.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2renzklpm.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2qcleetlp.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2kdxxgodf.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2ppdllovv.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2onehsqww.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2euofyygl.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2mokmhayg.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2kgqjloek.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2sltuytvn.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2razcozmo.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2kmvoxzrc.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2emacchqz.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2cksiwlla.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2dzcbdwig.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2hjvpjivo.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2klffolqj.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2swtadpsu.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2webuxkhj.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2sjrmpewc.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2ykqldnfa.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2nerwroyo.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2cwgyluff.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2wpiqvhbw.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2agdhmhti.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2cqltudyh.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2ezzkqhoz.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2lnllyyfv.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2tegbprtm.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2obmdqtew.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2gmfnguyl.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2pfqntpsy.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2lqvjajwp.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2fygcxxwq.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2fwxacdrf.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2zgpjnmre.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2uycqaitd.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2tuympfwl.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2tvgaakwa.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2nqwklmdr.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2rvddfbnl.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2uapcpcoh.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2hjjoivhe.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2tmgdmcci.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2uormslhu.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2thqsamru.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2vhottuxj.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2cnrkdinl.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2xsfcixqo.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2iqllwgwm.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2gprxmrfh.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2sdlfvcwp.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2ohsdaxnd.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2qcsyntao.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2eisxmlty.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2teqzbjyg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2onqdpukn.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2riquqaqk.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2kmydezfg.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2gsjbkbzj.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2hhpkxwar.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2kvuyyqbl.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2anqqutjd.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2ljzalpyi.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2mjvslifz.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2lypvugbp.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2wsjkavdy.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2msxovknd.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2hfeguqfv.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2zzhqdvga.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2cfskeubd.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2nhyatodm.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2zkujrykx.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2ogrfezyx.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2wpecdatm.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2iadequsk.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2bcywkrqm.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2gncznhat.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2annfmzdq.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2ctbvurqr.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2udtroslo.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2cxcaamce.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2bwccqaco.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2gptzwhdd.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2xzmefrnf.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2dnnmhcon.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2plxhykbu.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2yhdqeodo.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2pynucldx.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2efwqkjmr.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2xqbbycnj.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2vsfrifgc.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2vbkprrvt.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2ezbrjkrl.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2dlnidbvc.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2cksuvyge.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2cqvxsbcq.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2cegjwosz.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2fnqyzmzr.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2whzbrqit.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2yrjnvtui.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2dkxqleol.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2pxbrlqds.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2mjjwbmtg.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2hufmndqo.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2iitepopw.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2senylpvk.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2tuqjyroa.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2nxpfwnag.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2daosomlf.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2iernttlo.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2crqmibsp.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2zeywpitd.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2sbnaydsz.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2qspabsgy.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2rvhqduxx.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2nsltscsn.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2uygghgra.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2audingjs.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2bjkpgxqe.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2igqkaakz.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2lrofhjdi.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2gmfyffzv.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2gchfdobf.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2qobiptdr.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2nhkpgosp.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2xqknoouh.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2npxitwkw.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2pwmdkphj.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2vxjwrhsf.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2hkehdtqi.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2trowbcrx.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2omdawbeb.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2ouxwlfhf.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2ztxxghka.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2bewgwssi.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2qcwjjedg.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2byucoprb.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2yqabxyee.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2rsbxcmpt.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2pxnbrrgn.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2ssjkmdkj.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2syfdhwfo.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2ufayyxer.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2oxntfamb.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2fgbllkdx.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2zwzqaoqz.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2dvsqywdu.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2bobaniwh.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2frrpnqaw.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2gamdzybn.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2afartwok.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2wvussacx.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2jdpcycjy.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2ntbzjixh.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2xcdopsku.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2aomapeya.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2yhutcmcd.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2toacmhic.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2bpwxafiv.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2jbmwdbrn.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2syqfreys.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2yjopetuv.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2rgucnoim.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2kocvdlnx.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2gmhgvtzk.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2hfqnqiwi.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2tdkdksng.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2cnkmzhxu.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2nhlnmbgj.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2kizwfrca.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2uwxagqcn.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2nqpfhczf.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2hmwqrwpg.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2wndmcdgj.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2eadahfkd.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2lvajgeml.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2nwbwqyul.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2qhytsjln.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2bnpqshdo.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2xttwlaqq.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2xwlvqzhl.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2nkolsjmr.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2zuzbrces.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2zgvlukuu.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2eotemmwa.html


<!-- 参考信息 -->