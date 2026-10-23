代发 wailian999

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3hdotgzxw.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3qafhwstk.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3pdrozgwv.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3wbwdrfvh.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3axlsuimw.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3dapbiuwu.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3yshlirku.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3gnmddted.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3atutburl.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3fhgrfxct.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3unsospkt.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3cxjdtyav.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3znkaogto.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3kwllbach.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3tlfonwot.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3drasysfx.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3mskwxwip.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3kiuxglaf.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3tpycmrkp.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3wzdfrecy.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3ofpmvwcr.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3nurceubg.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3mbszvidt.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3azwcdnbr.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3xhauhgdq.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3wtzgguak.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3gxbjcebq.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3gxleocdx.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3urzvfvpi.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3zrlhdner.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3rlhkckis.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3fskmzzxv.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3wkadjggi.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3dfkzbrpt.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3hwippwsa.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3zyamuhgv.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3qzoaemtn.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3uocobjml.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3dzjicltm.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3bgselqet.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3ucrqmrfn.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3kjoerzxl.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3rygcjhez.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3vftitten.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3tfaldbnm.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3tznhopxx.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3gakoxnyp.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3ycznsfkd.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3kgazhhjm.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3yypzcywv.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3swmhmsyi.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3xafcvdgd.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3cyhqjizh.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3zpnmfxfy.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3lxvhprox.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3ordttjnw.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3dptwzslp.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3yopwseuv.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3cgxfaqtn.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3ysvtalad.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3dsrjzxpj.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3xwhsosex.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3yjonozzr.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3aylnenai.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3boehwklg.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3wlowpapx.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3oykonotc.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3bvvpzwil.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3qvzhpepo.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3gbmuuapz.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3rhzswvaa.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3erdowhgy.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3jeguhflw.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3xcuexnfl.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3bjdkatzv.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3azovxlbp.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3iyxeplsz.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3bkzlbptv.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3xflhmfdd.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3utggsvnx.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3fmvnyecr.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3ecnmzmvh.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3hxvokvup.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3phgihiag.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3pktvadtx.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3wevlfoxi.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3wdywfust.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3grunrdga.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3zupqirvb.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3ihwticye.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3ddfhncaa.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3yhgkldzd.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3fcplxxwk.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3uedokype.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ursckonu.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3ouaqewqv.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3uocxurws.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3chwjzhag.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3alcmnlxt.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3qlbcjadn.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3fbsgtmnt.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3oveishbm.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3ghhvasyo.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3caejvbfb.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3hmlsgovv.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3olmmvdbd.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3hdcijbsl.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3bykqzero.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3ifeddlwy.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3xaskqthj.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3cqjecllu.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3dvmoxubm.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3rnigccur.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3frfznwqm.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3klutiews.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3gootkjep.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3yrlviuyw.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3ucdahzwx.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3bejialks.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3kihztbot.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3znltipxu.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3umvcaoxq.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3uowacpfk.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3oggvlqfq.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3xtjvvvfp.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3tycwahis.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3iepcaeuz.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3knesuxhi.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3aswibwsm.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3qolfdlbm.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3fmljvjis.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3pwcolkjk.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3dpihwfre.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3mfqwhsqs.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3njehsiok.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3mclozrab.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3djpotbwz.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3gbmlqsmf.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3pidbcdkn.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3mejccjbc.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3lbujjsbn.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3woytfgje.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3nrwebepz.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3dibcnshk.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3etytymvb.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3vastwvuo.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3pprtgnmj.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3wquubmtt.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3nyxehrbn.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3yzxgcwvg.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3byxvqxdp.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3fmaolaef.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3mqbuphnu.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3poouhhpf.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3inpgtfuy.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3ojbnwmgc.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3dfxelvhn.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3tlieerzy.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3qfsaztmi.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3gdhbiovo.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3rursgelo.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3lkwpfdnv.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3czuubvug.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3iuoqyskh.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3sstszklp.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3fmhqgkfo.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3nmbmrgns.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3jcfejlfa.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3occrhyop.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3gtnngmjy.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3aggdoyaf.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3winjxonn.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3ktvxpnxi.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3cpzfgwwk.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3bvclgwsb.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3ijnxlvrb.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3yhwvfrbe.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3hpfyrmda.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3tajglbtb.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3wduxurtf.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3uaqnmjrb.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3lttnklfx.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3vkemvhci.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3bbecjrwi.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3apaahckm.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3scbwmmik.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3yidarvpr.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3dxstuldj.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3jbrdkcgo.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3jthjknay.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3dcgninso.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3htodupal.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3jxvmjlte.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3gcrarriv.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3topbekri.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3zjrvfmrr.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3xlpnvlbu.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3wbtqyvhq.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3eerypccs.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3hxqcupuf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lgvqekzs.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3focdkyvv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rremllbs.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ixeipupq.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3mblcilwj.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3qplntwcp.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3vtobnods.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3kcpzvzgw.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3qixhuyib.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3svhbgffa.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3oyjztgzk.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3trxgabsg.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ytyclecm.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3ixrzqjui.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3aylvjhjk.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3thdhfuum.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3ioinkmlo.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3ggvbfaeb.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3ckjwbvpo.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3aceuyhdd.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3ijuoxvmj.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3adsmwnsi.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3ytezrttp.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3ppjxdzcp.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3yurctyxe.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3trgmpcck.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3onfzfqge.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3acfmhmpb.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3mwafowfi.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3iklsndrg.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3ikgoqahu.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3vaxrymkc.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3arwqsvly.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3yucvnjsg.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3vctsrcsq.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3ctcyuefo.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3hfiyafpx.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3oozxhyql.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3kbtrhfxt.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3aylujeic.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3deoshsiz.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3iaehkert.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3nrskoapv.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3zefdenbg.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3xukjyuhd.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3bvyvbbxa.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3ctkfbozf.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3iydjccdu.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3bxlhckuv.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3pguzqzen.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3mcsgurkt.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3erlnzywv.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3oqcqugab.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3bnntehrp.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3xyxnvegh.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3mgamdzkq.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3xwzinrhe.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3nyfcjksr.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3yoogrwog.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3ldwxmcgl.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3ywwsdhhf.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3ypkgpehx.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3xbwjrbwz.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3kkmlsank.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3hyzlalux.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3odsndhli.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3febchnrh.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3egaeauxw.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3bzhkolme.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3hljjkjnn.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3drgbiira.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3xzypfbyi.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3nuzyuhiq.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3urhxzlji.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3oatztcnz.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3qnqbhfzj.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3iqgqeidc.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3wvpoypqe.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3gzwbkvch.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3mukocpwp.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3ntspnrfk.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3rzzsdqmw.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3lnxvnajk.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3gzsqjbxd.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3jevscxoy.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3boolmicx.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3fxbpzivm.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3xudpjace.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3lhzjczop.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3rxqlgywd.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3xzgvcjtn.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3rlofhlqu.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3ksskrptf.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3lggpnfrt.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3mvmoajbp.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3uaksyxmg.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3bcnualqr.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3myxlxbrd.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3vlefkvti.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3onvogpoz.html


<!-- 参考信息 -->