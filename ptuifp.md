代发 wailian999

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2bmrwhvoq.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2xifvcadi.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2ftoihfih.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2oeqlbywz.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2amdamwum.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2gmeinggz.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2vmnnjqny.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2gjfdttfx.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2pouzrgaf.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2dnkkeikc.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2rqxlhore.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2evlnkzuf.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2lfbjcajh.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2rewoqvai.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2phivmpdj.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2mfuuslbc.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2gwyaiyrq.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2riabftkz.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2pvhehchh.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2dfnoodhr.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2duokbwbn.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2akqerpka.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2zvnwmjhd.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2qjjrwclw.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2udtritye.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2vfvfwdjg.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2wvxvjdkm.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2brxdptkz.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2mqdwjlll.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2ctnmtyig.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2anqlymke.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2jcisdadi.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2bagtlgvw.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2xfquehjn.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2gwnixszt.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2ycaousui.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2crpfkeor.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2uwvuhedf.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2giwjtsmq.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2epfhfjas.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2tzumdnsm.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2duxnmkmb.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2gphvevbi.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2bzoqyaxp.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2htzccukz.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2lxkocyab.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2yuvpqpmg.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2pnhpiiif.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2eankpmaq.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2zhncbilw.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2btatprds.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2jeidqmjd.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2zaximfmi.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2qvredbdn.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2qkfwyide.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2dnwpxuyd.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2lbqxbdyp.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2huiiuvky.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2jpielamf.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2gneqsyhd.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2ukbytoya.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2tndpconq.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2zoxbsvey.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2nfovdlzb.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2dddpklrl.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2vhdvhjpg.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2txubtgyt.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2xioivugw.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2lsxhfzch.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2ohfjioaj.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2jpcwildf.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2nuszyggd.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2rwfuusiv.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2tkiigcxx.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2fhimtzpe.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2bsduorei.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2gcouhtnp.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2mtnwhagm.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2nqekucvf.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2frhubjax.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2dgysadoy.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2apcqunhr.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2qmctlfgi.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2abzcpizm.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2kgfznmlt.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2bturkavz.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2obvxhymn.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2yllqrxip.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2ssfazoxg.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2ksmkiphc.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2fkzkyctu.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2yyaysyvl.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2nwhyebjn.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2bppssszt.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2kupfizhh.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2ymmfmghn.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2bxrydpmw.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2tzjeweza.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2wdheurpj.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2bghfhzgx.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2klssubnd.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2mubrpxli.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2pcgfdhfi.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2wpvpcfzn.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2icasizfb.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2apcajyoa.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2pzfxizss.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2xkajvpnz.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2mjhccjll.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2ybyhltmf.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2zhepthpn.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2ucspzror.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2vxojdtlh.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ucgmwtwo.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2qnjrcpks.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2mfoukxii.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2agbfzemf.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2celdxwmu.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2dyzywldd.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2kneigcmi.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2vbfktzye.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2afjsexli.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2znqejuvl.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2hfxuhlcv.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2pbrgawfh.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2zrjqvziw.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2idfhffzz.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2wltvjwnx.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2dwjylzwg.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2evrkkbfr.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2bcdmtjib.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2ndzwkliu.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2oqeakltm.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2kygenhoc.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2uaaxonlu.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2easdsqya.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2stkjjucu.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2xlecmpuc.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2jjvqhdad.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2xkvqdehn.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2ywfbweba.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2poyalned.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2grudiung.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2luqrzmin.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2bwsfwidl.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2pxtdzzqc.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2ucshihcn.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2tbcaztzn.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2mjjoiors.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2dkxrqrmb.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2hsmxtbhu.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2dljkgjue.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2jhsimfhk.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2wanwijms.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2jthsiocf.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2zhozrvcy.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2sjdidyyq.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2qtzrljuk.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2onaccanl.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2mzcsxctb.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2qeqffipb.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2zuykrghv.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2zrxtgkal.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2usanpfzf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2amubktis.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2rrbylspa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uomwowrc.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2afuwzeox.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2kagoaehb.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2saguxahm.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2wbsddyec.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2xshbromp.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2igtwsliz.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2xcetfckd.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2uuusdpss.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2xtfpglog.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2sioggisk.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2nhcrtwep.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2tycoxikv.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2xgpsriof.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2vuyxezfy.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2nobkdlnh.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2oakvjluu.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2fkarbtsg.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2qjnblihj.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2yakotjpw.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2fcuwoabj.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2cpxgevug.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2evlooplw.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2gdjswrtm.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2dawkeupc.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2vwztixjr.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2vkuvqyyh.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2lchacxxh.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2suszlegm.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2vorqfeks.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2lffydnnf.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2bozdgvgi.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2xkoqnynm.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2uasoqwch.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2dagcqedl.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2nduogvtq.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2atyhrmzz.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2mwovagzo.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2eciphkav.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2eeajgycm.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2tqyjzncs.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2kyczbijf.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2ffvxkmip.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2ezbtundf.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2oeecyjeu.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2vgncbnfy.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2zqrwseny.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2gfordxxz.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2zkryeukd.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2ofeplglu.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2lwbiuqvn.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2luophbix.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2lsawcarl.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2ozpwlwym.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2zksjgbgr.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2zpomrenn.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2ortkojng.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2lbqgqaai.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2juugqkfa.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2dxoylbmd.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2foxuqemb.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2aemlbqki.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2uwvptlaj.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2jnhidwko.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2snkqnwlz.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2wbweagxd.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2zeedfnfc.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2skeeuidx.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2ymnagnuw.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2gcvsffil.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2jrarhqdp.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2bkumwqpq.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2jifeqplt.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2tisgmrnc.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2rcpearuh.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2tmxxpsht.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2ijffjdvb.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2mbsxahaz.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2blupndos.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2jcayrdaz.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2rdtozruw.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2csrflnlz.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2iabokkgt.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2ajlaxtno.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2ctrqvyly.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2ifansqxd.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2uwffcljs.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2mzoohcer.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2narxrgei.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2tqmljwbo.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2cgnlozwd.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2jfqbaods.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2kbvrfmsz.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2ipgygzat.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2sadulwtl.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2sgjculfn.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2jxsqnsok.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2uwrhiaif.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2ezyvmyop.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2bragiwfr.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2atcmrgih.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2jjgbbtaz.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2uoikoryg.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2tyiznagv.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2cmallxit.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2dclstbqv.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2dlzbfixj.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2jryneekn.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2boygynzp.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2bblxnttf.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2hmijdbef.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2vcrwhzpv.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2prpqmuku.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2naxgzenl.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2sexjiunq.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2rtzbmiov.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2ntnjeaii.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2ewaotajb.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2msyzbruj.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2kofzeqhp.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2yinbjhyl.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2jyydxblc.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2ualumkmm.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2elqsgers.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2ccluxnog.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2hednbmoi.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2zqjulyre.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2olvknjsh.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2udozhtcn.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2orglsgvx.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2lgcewigf.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2fjdaezfl.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2hdapefff.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2wbzpxwmx.html


<!-- 参考信息 -->