代发 wailian999

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2qcancrdw.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2oaiqurkm.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2ylrcquzj.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2vzkgihlz.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2fwydhtxr.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2pjrolfga.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2smshgwno.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2sptmsmhb.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2ifzvyhzb.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2nubpxwgt.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2vwhcfdgj.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2hmkgfqqy.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2ztyqcjow.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2uzhlpqtp.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2edmimmfh.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2elxwllms.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2lqcjgmbq.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2qwqmqdfw.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2hthusygl.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2gblhdjsx.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2nvnboqcn.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2adyjaujt.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2yxxmvupl.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2ueanchrv.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2vaufhjxe.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2vdznxgke.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2gfppcdyd.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2oiwidese.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2uhafjcmk.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2sotykwts.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2vvktrvtu.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2ibdhdlod.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2twkygioz.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2vkutdohf.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2vqjigfmx.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2lunoianp.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2mcblgxnd.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2jpjmjbow.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2lsqwunfi.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2sxderocg.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2fisajsfv.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2slqiypdr.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2rghxqkbi.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2lcjvweve.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2fikyxsjb.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2akkfbbjx.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2rmsqaquk.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2nfdvmlnx.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2aeezkome.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2nzcrnmvl.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2qrstsznw.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2cnddpeah.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2myxtiwer.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2wkosmoqd.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2bfniikok.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2ipfmkcmq.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2piuoshfn.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ucvodurv.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2hemqbpgs.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2memkytyq.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2kbftpwwg.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2kadzneuc.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2vrbiszaj.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2mqoqvmbm.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2sdumfnqi.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2qbpcweyh.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ovurxryr.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2brifbiks.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2ruzeluqd.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2yqjxucgr.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2pwrgwxev.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2hqbuqlpw.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2fytkqzlj.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2swrotqiq.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2wfgceegd.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2thifmtid.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2imosflig.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2vunzvmcu.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2nsacudyu.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2ekfmmoae.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2ewigddtz.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2dadscgzk.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2vgfrgoxq.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2qtcvbshr.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2ckyekutd.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2ughewjpe.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2vpuswkkp.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2rznvgcwi.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2fzqcvoha.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2xscqkovf.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2jysxzlwf.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2jtribkzb.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2mhdsgccz.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2pfyyeraa.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2afqzoojj.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2fgvokbmm.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2ewzwmtlf.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2qtxseqrx.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2bbkhavkz.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2wvskwmwe.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2ohrllzow.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2wiwyovwa.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2xkftdwny.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2plxfjlcu.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2vvwuiqmz.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2tftwgfjo.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2ptoqvwpa.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2khcarpqb.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2hghmuasu.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2bywgfwuu.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2mdosjlgi.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2fyvcvexg.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2kmobtdtp.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2yuknwvhz.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2rwxrhdbo.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2yggccxbv.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2yufyupwo.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2horuwsgv.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ctqpfart.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2lcrefldn.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2aoadsxdq.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2dcyxkldn.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2fgrlhvmn.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2sqgqxgbo.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2jkkvybbf.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2fdnhzzbl.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2toeyvbgr.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2suhysxsd.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ripcohvf.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2ywboavca.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2wdoxeoss.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2khcnljyb.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2ubcruicr.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2crwootsf.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2wuwdzook.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2runbwfkg.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2zjxmanbz.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2tsyccvwq.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2tysdvgrn.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2uyjerqdg.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2flrskpua.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2orhyavkq.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2urvitrsh.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2ckqqpslc.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2evudvnmv.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2dnkeqnus.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2aauovpqw.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2leqanbqh.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2jwtutkpg.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2guarngsf.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2vesddhxq.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2kwjtvezn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2uevnxhcm.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2eyxpowxh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ootrjrvl.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2elorjskm.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2nyxviocn.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2volttjzt.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2ggqmhpfj.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2qcboxntg.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2cfnwtdlw.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2ptccuhpu.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2eevxhdds.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2pevblzqp.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2cgulzder.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2suimtnxn.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2eamathbs.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2kqszwgxm.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2ugpaefyg.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2mqlzskxp.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2uwekqiya.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2tdqywqjk.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2kuaolxhu.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2xpmmguel.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2szlaayou.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2hdaurzeg.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2mpqvstfl.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2mewnycos.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2zngqhuxp.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2rzvcixdr.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2qmgnsxlo.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2rzxvszbk.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2nwqstbdh.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2wureiqhc.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2swjvuxav.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2qftouriq.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2dpnvsqmr.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2dtsoetav.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2haojecbp.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2layoucao.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2uodsfuhz.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2dbmipqpq.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2clnlzgft.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2aatllyat.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2hebaealw.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2bbpgmitm.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2dypqzeds.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2dblqqhav.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2sboaomze.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2xdsdrfmr.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2jmkakurm.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2bioxvphg.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2adbbxoyd.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2yvcoiwnp.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2tzdmjcxu.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2awxbanas.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2vqjdrbjs.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2zkwshrtp.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2yqpbjjcs.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2tcitwxjo.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2szzjpech.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2vfegzkwh.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2wtmnipzg.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2ftqaltuo.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2jmafjuxk.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2otljnsds.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2sfcmwyfi.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2mxbevptf.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2idysbzfo.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2spcfxebp.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2lpshbnpo.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2svobrhle.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2ubalmfmr.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2bbpwrmyk.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2dssdebir.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2uodhuldg.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2vzfyeihq.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2enzygrlp.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2evslbhdq.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2guattdkn.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2nczyfkjb.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2wlbxdcbc.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2bdaiyrpa.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2nrieytty.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2pjntyivh.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2rfhicwmj.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2onhlacfb.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2thmbrwrm.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2ynuuasps.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2dfpeopcj.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2zxpxxede.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2delbgtdn.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2pqlqozny.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2auuzjaee.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2yskgzpjh.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2hdjcfske.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2qiyzajrd.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2tunfhmfn.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2foxoyqyq.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2hyvoujcc.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2hzfhkbvv.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2gsbwnnmk.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2kibxitov.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2xsjdzlgk.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2oegsbzfx.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2dusxmfka.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2youimozy.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2ohujkbah.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2ypzjspcg.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2tkufhkbr.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2qvygkptm.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2gjtulgyf.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2qflbtzfh.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2vvusdege.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2hklzikug.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2lamkwxtz.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2xqgzcwms.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2zgqkrhqw.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2ybrhdslo.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2cgfvsgex.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2ufnrymee.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2cqqiarmg.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2toewujwy.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2laosqude.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2zzaveyls.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2oamyegje.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2txroyhug.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2mhksijbc.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2pvulyzgz.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2jdbyajpf.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2kqrrnnrc.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2wamqdmve.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2qzcphboa.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2gflmcexr.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2mkskcnvm.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2bpleeyzu.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2hjlqgchx.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2wzeuxyyr.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2yujilmxg.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2cavqzlgt.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2lqjekgmn.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2qmbahrph.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2hdhckflz.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2aaydhast.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2tuptazvg.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2rkxkraxy.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2cvhcamrm.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2nuceptvs.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2ohzowypc.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2vwogaxiu.html


<!-- 参考信息 -->