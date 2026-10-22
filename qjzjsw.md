代发 wailian999

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2hxawnrqb.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2epgqxmqg.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2bvxdiyuw.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2ajzbbtkw.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ugnoomlm.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2tlkyxicp.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2jsanjgae.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2yynvnrok.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2iojfjppo.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2jxqfblpf.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2krmqvzya.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2zordnpvz.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2rpolhpeo.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2anbrixsk.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2alohuvkk.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2jzkokcoq.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2rczkewin.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2xvlfgwhu.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2eblisxpr.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2zwfegbds.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2rmkpazgs.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2bdpfuigf.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2hklajpwf.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2bqekzera.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2pnpwlmxe.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2ctgqnzpu.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2komwokhp.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2wumrskoo.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2ahskzvfh.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2rwnikoal.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2seupzhgs.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2tfijeazu.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2hermagfs.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2hgjsbpjn.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2ujtvkiwb.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2wjzsanjw.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2hbsmloif.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2cmtonugv.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2bcgnksxj.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2owwxbuun.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2kftwqznt.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2fjigyubk.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2hgzkxpsp.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2oqmeukqi.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2pfsfivxt.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2xzzukbcy.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ionsxeyv.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2dqumtvbl.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2zfkaefbe.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2vfndsjkl.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2vzvblnmq.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2dvnszngs.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2cbujwmbe.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2qmbntedm.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2gqakvmfo.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2bnajbzay.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2tygirnll.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2hkisgldn.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2cziysmqr.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2nthngvgy.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2spbctmip.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2rcaxkzil.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2shvmyjsf.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2zjsnueul.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2huirujsb.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2frapojli.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2ekbrbbci.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2drtqfdkc.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2oxognahi.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2psctwjqn.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2jxgvdhbk.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2xdxyyhvv.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2puzujykm.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2xsuhjome.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2hddnzadu.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2xwjjguwc.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2dyovjozl.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2mdwaeftv.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2nrfhevfx.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2bzugwoir.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2rawyafvp.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2foyocdro.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2nkkcigph.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2cvgkkzoy.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ckcuknlb.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2tgihdztg.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2wpfvkafj.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2selyzufk.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2ioupccch.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2yfpghddw.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2kyftgguv.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2pcccgfqr.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2gcedkevi.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2gkxevjjg.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2jmpldvsc.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2ugrpaddz.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2vcvkrkhs.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2npaqcvvm.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2eamxsuap.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2msrdvxkh.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2qgwmuyds.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2cutnazgk.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2nptrcukl.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2egrrrtyf.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2rslvmjew.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2msgvijje.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2cdyjitvg.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2ioieyshd.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2przeqfzb.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2wzcbqvip.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2gzvzenyl.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2voryiiet.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2yxxonmks.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2fhecdajm.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2wwqmdnzu.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2jtlkfhcv.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2gxrmuhtm.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2gbdsucgy.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2yjvxhbxb.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2xtvjoshy.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2jzunbokb.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2mooanrtp.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2zagcgiaj.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2briwteon.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2dtselxsr.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2uukdbgwu.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2gibttpwx.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ocsemzki.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ztadxpod.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2juznvztj.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2ykrvzgan.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2voigcacr.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2fbxygfjx.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2rtzngttg.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2sitdclxx.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2fttqkeki.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2qgktlppe.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2jkkustuz.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2ytsrbfwv.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2qxrvwbbo.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2dsixtpss.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2sccxwdgk.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2jksdzyrc.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2ddxdtpka.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2esaureze.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2juvjppue.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2igkaliai.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2dsrrldpi.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2enkfigid.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2hvuvrxxi.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2joxcjivs.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2vjhhwxzu.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2ydqcbhkl.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2uakmrzwi.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2hsqtfluf.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2ahwqvrfw.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2mqtafvso.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2ozbotlnz.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2mclgadmi.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2ekqgfieq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2sygdubkc.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2ikvtwibe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dfbpyqwq.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2ytjoiaim.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2usylfqao.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2igalxibg.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2opcgetei.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2spchfqbq.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2uaiqmorb.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2dnusfqac.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2jwepciff.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2lqzgoxgv.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2lchvrsnm.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2rsjefsba.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2ilukkwqa.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2mmfzkhmp.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2xxhczupd.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2bsfrtsga.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2vyscqose.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2apkhvauv.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2weekjspo.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2fjsucshw.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2gdffzelt.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2jdbfqshj.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2ezdnbzgq.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2rwfqgaff.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2bmbtiokx.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2pxvxikdr.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2udtqgxew.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2qalpudqy.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2umibwuab.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2zmlxmikn.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2zdkcadme.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2kbegcohb.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2znsbqazm.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2bigemqbd.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2ofomezqx.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2ssgvlmqs.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2nctyisyy.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2xyodjwiv.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2uxbykgvx.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2thrfzofv.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2erpsslns.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2gxirhnoo.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2jggoccii.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2cfyhntvd.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2krcgfpuk.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2wwozlhye.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2ummqmnlg.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2runjrzvu.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2lkfzfblw.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2svvjsdgc.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2xwxaache.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2srlcwzeb.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2trbhsdvm.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2fyrrfhmu.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2sgximvpi.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2yfzadhrn.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2tclfcstf.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2svkiayny.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2sppujswi.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2hwkqpjnx.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2ztmgmicl.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2utmzohdk.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2mkhcxejq.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2tqxfbemb.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2kqdcrigt.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2wxyqitxe.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2qoguryqu.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2pqrpzksi.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2lesfpcjc.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2cknzvvbw.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2vkdfntbr.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2gnsdgyxm.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2jzesjruy.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2jdzuinfo.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2vlreqkek.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2jusgejxx.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2vwcxyskc.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2vkwuwbsx.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2jcymfxqu.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2vbclyzge.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2oupbesqm.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2aaqvkeaa.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2ufvvxdqg.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2ebyhcaap.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2sgannqez.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2iyctnstn.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2gofmsvzl.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2dhobymzy.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2ikwxcrfl.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2ngkesedp.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2xsotamtn.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2mdsbkyvs.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2zymzjeuy.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2dhsmiahc.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2qjpoczcv.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2vtlfldpu.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2vwrwquun.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2odjiemki.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2senqupxw.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2zgggxbgq.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2dqkyefis.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2fvruqycc.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2gauvnatz.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2lophhrhb.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2dqreqmpn.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2fhytzkci.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2qeuuzevs.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2ctebwsbz.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2mvplfxrg.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2oahftrln.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2zmesoffq.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2awamgvqt.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2ugvgbpek.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2gmtrhpmf.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2bckegcdu.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2usoocbqy.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2jpfbrgoe.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2sndoennm.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2cuwgdkjx.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2dcpvpmbq.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2moszgksn.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2witcudln.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2nikxocpp.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2pvucyofs.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2htyohzdo.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2ldwdmwtd.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2bgwayzkl.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2zhlrduyp.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2iexhflsu.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2vphcilfg.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2qhynxyui.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2iypwhbux.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2woitytmj.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2foharrbt.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2vemrkuew.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2kdtwgihi.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2vnxvomzv.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2gmaxigui.html


<!-- 参考信息 -->