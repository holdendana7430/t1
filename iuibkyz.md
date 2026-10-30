代发 wailian999

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://m.share.zdbjq.cn/Article/details/gckzsqpvu.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.hesvh.cn/Article/details/gjbokwjjv.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.zdbjq.cn/Article/details/ggelgbsnm.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.zdbjq.cn/Article/details/gqnejchao.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://wap.zdbjq.cn/Article/details/gqrdbttdp.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://m.share.fehbvm.com/Article/details/gcdcukwxs.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://baike.fehbvm.com/Article/details/grylvfllt.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://3g.zdbjq.cn/Article/details/gsliopbvf.sHtML

[D11] 反转数组
来源：http://wap.hesvh.cn/Article/details/gndvovlek.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.blog.zdbjq.cn/Article/details/gxsadppsw.sHtML

PHP:  array_reverse($arr);
来源：http://baike.zdbjq.cn/Article/details/gpgstwpax.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://blog.zdbjq.cn/Article/details/gtshrxetw.sHtML

TS:   [...arr].reverse();
来源：http://baike.hesvh.cn/Article/details/gzsnfjakf.sHtML

Java: Collections.reverse(list);
来源：http://www.blog.fehbvm.com/Article/details/gqwwahoga.sHtML

Go:   slices.Reverse(arr)
来源：http://m.share.hesvh.cn/Article/details/gkjgexjup.sHtML

Ruby: arr.reverse
来源：http://baike.fehbvm.com/Article/details/gqzcmresg.sHtML

C#:   list.Reverse();
来源：http://mobile.zdbjq.cn/Article/details/gryhlzrgd.sHtML

[D12] 查找元素下标
来源：http://www.blog.hesvh.cn/Article/details/ghdppnuut.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.m.share.zdbjq.cn/Article/details/ghixgzhqr.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://baike.fehbvm.com/Article/details/gyxlfjqdz.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.fehbvm.com/Article/details/gazrrkqyv.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.zdbjq.cn/Article/details/gurbburcv.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://blog.fehbvm.com/Article/details/goocuaouy.sHtML

Go:   slices.Index(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/gjgokjngz.sHtML

Ruby: arr.index(x)
来源：http://www.share.zdbjq.cn/Article/details/gwcicswpz.sHtML

C#:   list.IndexOf(x);
来源：http://www.m.share.fehbvm.com/Article/details/gdklgmvxe.sHtML

[D13] 过滤（保留满足条件的）
来源：http://read.share.zdbjq.cn/Article/details/guhwdykxk.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://baike.zdbjq.cn/Article/details/gxgxcxuoa.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://blog.fehbvm.com/Article/details/gwtuzaotw.sHtML

JS:   arr.filter(x => x > 3)
来源：http://baike.zdbjq.cn/Article/details/gcshmwwhs.sHtML

TS:   arr.filter(x => x > 3)
来源：http://blog.fehbvm.com/Article/details/gkccvagve.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://blog.fehbvm.com/Article/details/gnwakswdg.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://wap.zdbjq.cn/Article/details/gixkauvqo.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://mobile.fehbvm.com/Article/details/gktdibhuk.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://3g.fehbvm.com/Article/details/gffawkoqx.sHtML

[D14] 映射转换（每个元素变形）
来源：http://mobile.hesvh.cn/Article/details/gsligfita.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://baike.hesvh.cn/Article/details/gooyedboq.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://read.share.zdbjq.cn/Article/details/guneckypd.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.share.fehbvm.com/Article/details/giphlxqke.sHtML

TS:   arr.map(x => x * 2)
来源：http://3g.hesvh.cn/Article/details/gcdljihsk.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://mobile.fehbvm.com/Article/details/grrvapvwa.sHtML

Go:   // 手写循环
来源：http://www.m.share.hesvh.cn/Article/details/gebvupwdf.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.blog.zdbjq.cn/Article/details/gcctpyjdr.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://baike.fehbvm.com/Article/details/gfrvmatwr.sHtML

[D15] 去重
来源：http://www.m.share.hesvh.cn/Article/details/ggawmqpyg.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://wap.zdbjq.cn/Article/details/gptooawbb.sHtML

PHP:  array_unique($arr);
来源：http://m.share.zdbjq.cn/Article/details/gbavacaut.sHtML

JS:   [...new Set(arr)]
来源：http://wap.zdbjq.cn/Article/details/gwdeqksoi.sHtML

TS:   [...new Set(arr)]
来源：http://3g.zdbjq.cn/Article/details/glawpopqw.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://baike.hesvh.cn/Article/details/gdmicswhw.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://baike.zdbjq.cn/Article/details/gidxxxptr.sHtML

Ruby: arr.uniq
来源：http://www.share.hesvh.cn/Article/details/gtudtxbym.sHtML

C#:   list.Distinct().ToList()
来源：http://www.m.share.zdbjq.cn/Article/details/ghswhcwfq.sHtML

[D16] 求和与平均值
来源：http://m.share.zdbjq.cn/Article/details/gjbzkwxhl.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://mobile.hesvh.cn/Article/details/gjorkektl.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mobile.hesvh.cn/Article/details/gcotztlxh.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.zdbjq.cn/Article/details/giqxxvcwi.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.hesvh.cn/Article/details/ggwazskzs.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.share.fehbvm.com/Article/details/ggynxmqjq.sHtML

Go:   // 手写循环累加
来源：http://www.blog.hesvh.cn/Article/details/gfgwufdwa.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mobile.zdbjq.cn/Article/details/gsaovevbt.sHtML

C#:   list.Sum();  list.Average()
来源：http://m.share.hesvh.cn/Article/details/gotbabxte.sHtML

[D17] 最大值与最小值
来源：http://m.share.zdbjq.cn/Article/details/ghsluzkmq.sHtML

Py:   max(arr);  min(arr)
来源：http://blog.zdbjq.cn/Article/details/gotscoats.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.share.zdbjq.cn/Article/details/gfelvvebl.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://3g.hesvh.cn/Article/details/gkwrczkrq.sHtML

TS:   Math.max(...arr);
来源：http://www.blog.zdbjq.cn/Article/details/gasswinpn.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://m.share.hesvh.cn/Article/details/gybhfytsv.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.share.hesvh.cn/Article/details/gygpxqbnx.sHtML

Ruby: arr.max;  arr.min
来源：http://baike.fehbvm.com/Article/details/gokahbgmm.sHtML

C#:   list.Max();  list.Min()
来源：http://m.share.fehbvm.com/Article/details/gwchnmgck.sHtML

[D18] 扁平化嵌套数组
来源：http://3g.fehbvm.com/Article/details/gcvvbooao.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.blog.fehbvm.com/Article/details/gmjqoaijc.sHtML

PHP:  array_merge(...$nested);
来源：http://m.share.fehbvm.com/Article/details/ggnaywzch.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://read.share.zdbjq.cn/Article/details/gxigsqthd.sHtML

TS:   nested.flat();
来源：http://mobile.fehbvm.com/Article/details/gtzvjvjqu.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mobile.fehbvm.com/Article/details/gbbruoejg.sHtML

Go:   // 手写双层循环
来源：http://www.blog.zdbjq.cn/Article/details/gvggrfvjm.sHtML

Ruby: nested.flatten
来源：http://mobile.zdbjq.cn/Article/details/gkpvkfzgy.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://m.share.zdbjq.cn/Article/details/gbkmbegkj.sHtML

[D19] 按字段分组
来源：http://blog.fehbvm.com/Article/details/gtsddtyav.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://3g.hesvh.cn/Article/details/guoqmdghg.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://blog.zdbjq.cn/Article/details/gtujdfblt.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://3g.fehbvm.com/Article/details/genfxzvpd.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://m.share.fehbvm.com/Article/details/gneeqoash.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://read.share.hesvh.cn/Article/details/gqnyiatcf.sHtML

Go:   // 手写 map[string][]T
来源：http://www.share.fehbvm.com/Article/details/gkytnnssw.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://m.share.hesvh.cn/Article/details/ghngkquwn.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wap.zdbjq.cn/Article/details/ghptpeuol.sHtML

[D20] 统计每个元素出现次数
来源：http://mobile.fehbvm.com/Article/details/ghkowuyvn.sHtML

Py:   Counter(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gbrugjbay.sHtML

PHP:  array_count_values($arr);
来源：http://wap.fehbvm.com/Article/details/gbjtlkwmn.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.fehbvm.com/Article/details/giwdpqpox.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.zdbjq.cn/Article/details/gqyaijejk.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.share.hesvh.cn/Article/details/gaixfyfxh.sHtML

Go:   // 手写 map[T]int
来源：http://www.blog.zdbjq.cn/Article/details/gninlseib.sHtML

Ruby: arr.tally
来源：http://www.m.share.zdbjq.cn/Article/details/gajeidzvv.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://3g.zdbjq.cn/Article/details/galtkqtkj.sHtML

[D21] 判断是否包含某元素
来源：http://blog.zdbjq.cn/Article/details/gndbotbad.sHtML

Py:   x in arr
来源：http://www.blog.fehbvm.com/Article/details/gwepmcywf.sHtML

PHP:  in_array($x, $arr, true);
来源：http://baike.hesvh.cn/Article/details/gwsblivle.sHtML

JS:   arr.includes(x)
来源：http://m.share.fehbvm.com/Article/details/glvqpgzgb.sHtML

TS:   arr.includes(x)
来源：http://blog.fehbvm.com/Article/details/gphzqasof.sHtML

Java: list.contains(x)
来源：http://www.m.share.zdbjq.cn/Article/details/ggrhglfjl.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/gunoxxpvo.sHtML

Ruby: arr.include?(x)
来源：http://m.share.fehbvm.com/Article/details/gcxqmfnju.sHtML

C#:   list.Contains(x)
来源：http://blog.zdbjq.cn/Article/details/gdyztkcsz.sHtML

[D22] 复制数组（避免共享引用）
来源：http://wap.fehbvm.com/Article/details/gomugdogg.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.share.zdbjq.cn/Article/details/gltksjyps.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wap.zdbjq.cn/Article/details/gmnwhepub.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://3g.fehbvm.com/Article/details/gkhcyaxje.sHtML

TS:   [...arr];
来源：http://wap.zdbjq.cn/Article/details/gfisyqbpu.sHtML

Java: new ArrayList<>(list);
来源：http://baike.zdbjq.cn/Article/details/gcdmvnibv.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://read.share.hesvh.cn/Article/details/gfyevuvjz.sHtML

Ruby: arr.dup;  arr.clone
来源：http://wap.hesvh.cn/Article/details/guhpgtbuy.sHtML

C#:   new List<int>(list);
来源：http://www.blog.zdbjq.cn/Article/details/gifcvikhl.sHtML

[D23] reduce 累积计算
来源：http://baike.zdbjq.cn/Article/details/gdzlnyzhx.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://3g.zdbjq.cn/Article/details/gbtznhjos.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://read.share.zdbjq.cn/Article/details/gsewqcqxf.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.hesvh.cn/Article/details/gppgoscxr.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.fehbvm.com/Article/details/gemfzsyrc.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.blog.zdbjq.cn/Article/details/gztugiyrk.sHtML

Go:   // 手写循环
来源：http://www.blog.hesvh.cn/Article/details/gpndqpawb.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.blog.hesvh.cn/Article/details/gfecqolnq.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://blog.hesvh.cn/Article/details/gsovnbegk.sHtML

[D24] 字典 / Map 基本操作
来源：http://baike.hesvh.cn/Article/details/gebxchzpf.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://baike.fehbvm.com/Article/details/gwrmjnxgr.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://3g.hesvh.cn/Article/details/geogmigrc.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wap.hesvh.cn/Article/details/gccyjghbp.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://mobile.fehbvm.com/Article/details/ggspswczc.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://3g.zdbjq.cn/Article/details/gfsjfiisc.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.m.share.zdbjq.cn/Article/details/glfymadij.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://mobile.fehbvm.com/Article/details/gcymgyche.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://3g.hesvh.cn/Article/details/gouimvhpc.sHtML

[D25] Set 集合去重与交并差
来源：http://blog.fehbvm.com/Article/details/gvjpllttk.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.share.zdbjq.cn/Article/details/gvdzubsmd.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://blog.fehbvm.com/Article/details/gizrckdux.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.m.share.hesvh.cn/Article/details/gdbauiwkq.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://3g.fehbvm.com/Article/details/gfxkargcm.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.m.share.fehbvm.com/Article/details/gfuvwixrm.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://read.share.fehbvm.com/Article/details/gtutpktly.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wap.hesvh.cn/Article/details/gjgxrttqy.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://baike.fehbvm.com/Article/details/ggybaujyz.sHtML

[D26] 数组转字符串
来源：http://blog.fehbvm.com/Article/details/gvpjxkghm.sHtML

Py:   ", ".join(map(str, arr))
来源：http://3g.zdbjq.cn/Article/details/gyjukpgdh.sHtML

PHP:  implode(", ", $arr);
来源：http://wap.hesvh.cn/Article/details/gpjnqffdb.sHtML

JS:   arr.join(", ")
来源：http://blog.fehbvm.com/Article/details/gpmwrqoqe.sHtML

TS:   arr.join(", ")
来源：http://www.m.share.hesvh.cn/Article/details/gimocuaoe.sHtML

Java: String.join(", ", list)
来源：http://blog.hesvh.cn/Article/details/gjxgfdvzz.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.m.share.fehbvm.com/Article/details/gpuowumbu.sHtML

Ruby: arr.join(", ")
来源：http://mobile.fehbvm.com/Article/details/gszopjzqv.sHtML

C#:   string.Join(", ", list)
来源：http://3g.fehbvm.com/Article/details/gcihsdhop.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gomiuqfod.sHtML

E. 字符串处理
来源：http://m.share.hesvh.cn/Article/details/gzcbtoxjv.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gdnwplteh.sHtML

[E01] 拼接字符串
来源：http://read.share.fehbvm.com/Article/details/gipitqvpi.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://mobile.hesvh.cn/Article/details/gltcyyuth.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mobile.hesvh.cn/Article/details/ggojhexkg.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.fehbvm.com/Article/details/gliggmygl.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.zdbjq.cn/Article/details/ggskghhku.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://blog.zdbjq.cn/Article/details/gtxjyjtro.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://3g.zdbjq.cn/Article/details/gblrqktqh.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.share.fehbvm.com/Article/details/gkxhypfxn.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://read.share.hesvh.cn/Article/details/gglhjjhjd.sHtML

[E02] 重复字符串
来源：http://www.blog.fehbvm.com/Article/details/gvngnxpkm.sHtML

Py:   "ab" * 3
来源：http://3g.hesvh.cn/Article/details/ghpitndmz.sHtML

PHP:  str_repeat("ab", 3);
来源：http://read.share.zdbjq.cn/Article/details/gxkihcqcx.sHtML

JS:   "ab".repeat(3)
来源：http://blog.hesvh.cn/Article/details/gyofhctvi.sHtML

TS:   "ab".repeat(3)
来源：http://blog.zdbjq.cn/Article/details/ggnanjyjc.sHtML

Java: "ab".repeat(3)
来源：http://mobile.zdbjq.cn/Article/details/gwhpueiqf.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://baike.fehbvm.com/Article/details/glanwaiqr.sHtML

Ruby: "ab" * 3
来源：http://baike.zdbjq.cn/Article/details/gfurgcsti.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://blog.hesvh.cn/Article/details/gqgpgexue.sHtML

[E03] 截取子串
来源：http://wap.hesvh.cn/Article/details/gdyvoxkee.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://mobile.hesvh.cn/Article/details/gqnofimio.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.m.share.zdbjq.cn/Article/details/gacfpwskn.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://m.share.zdbjq.cn/Article/details/gsemfzkvq.sHtML

TS:   s.slice(1, 4)
来源：http://wap.fehbvm.com/Article/details/gfsnkrnju.sHtML

Java: s.substring(1, 4)
来源：http://3g.hesvh.cn/Article/details/gpjziqxdr.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://mobile.zdbjq.cn/Article/details/gavkjgcjc.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://wap.fehbvm.com/Article/details/gqyimqumd.sHtML

C#:   s.Substring(1, 3)
来源：http://mobile.hesvh.cn/Article/details/gxsfkhlpf.sHtML

[E04] 查找子串位置
来源：http://read.share.fehbvm.com/Article/details/gnlnflpvm.sHtML

Py:   s.find("x");  s.index("x")
来源：http://blog.hesvh.cn/Article/details/gheealfti.sHtML

PHP:  strpos($s, "x");
来源：http://3g.zdbjq.cn/Article/details/glmkonnqg.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://read.share.fehbvm.com/Article/details/gjxbdwjju.sHtML

TS:   s.indexOf("x")
来源：http://read.share.hesvh.cn/Article/details/gwdyfhgrd.sHtML

Java: s.indexOf("x")
来源：http://www.m.share.hesvh.cn/Article/details/gskbaijcl.sHtML

Go:   strings.Index(s, "x")
来源：http://m.share.zdbjq.cn/Article/details/gotuqkxnj.sHtML

Ruby: s.index("x")
来源：http://wap.fehbvm.com/Article/details/giznellvd.sHtML

C#:   s.IndexOf("x")
来源：http://www.m.share.fehbvm.com/Article/details/gmhvoenej.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://blog.zdbjq.cn/Article/details/gwceekwho.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://baike.hesvh.cn/Article/details/glrpxpvkz.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wap.hesvh.cn/Article/details/gioqcekfc.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.zdbjq.cn/Article/details/gassmedzz.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://read.share.fehbvm.com/Article/details/glygwgjgl.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.hesvh.cn/Article/details/gewwoxhoz.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://read.share.fehbvm.com/Article/details/gdcmfhmnu.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://wap.hesvh.cn/Article/details/gewobqzsw.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.blog.zdbjq.cn/Article/details/gqqgmljdv.sHtML

[E06] 替换子串
来源：http://m.share.hesvh.cn/Article/details/gncsicalr.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.m.share.fehbvm.com/Article/details/ggvgbaczw.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://mobile.zdbjq.cn/Article/details/geyyitqwe.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.fehbvm.com/Article/details/glrrabrwb.sHtML

TS:   s.replaceAll("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/ghehnyxys.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.fehbvm.com/Article/details/grftwgwpk.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.m.share.zdbjq.cn/Article/details/gfaefixss.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://m.share.hesvh.cn/Article/details/gyjngyqgr.sHtML

C#:   s.Replace("a", "b")
来源：http://baike.hesvh.cn/Article/details/grfyvsfwk.sHtML

[E07] 按分隔符拆分
来源：http://www.m.share.zdbjq.cn/Article/details/geeabgigp.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://baike.zdbjq.cn/Article/details/gwvszbmnd.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.blog.zdbjq.cn/Article/details/ghwoaaocb.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.share.zdbjq.cn/Article/details/gztvamiaf.sHtML

TS:   s.split(",")
来源：http://www.share.hesvh.cn/Article/details/gayxbnmaf.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.blog.zdbjq.cn/Article/details/gtyhonrbs.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://mobile.fehbvm.com/Article/details/gxzqnjsvv.sHtML

Ruby: s.split(",");  s.split
来源：http://www.share.hesvh.cn/Article/details/gpogwgoeo.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://read.share.fehbvm.com/Article/details/gptkbytsl.sHtML

[E08] 数组按分隔符合并
来源：http://3g.fehbvm.com/Article/details/govietjdv.sHtML

Py:   ",".join(items)
来源：http://baike.fehbvm.com/Article/details/gexmlazaz.sHtML

PHP:  implode(",", $items);
来源：http://read.share.zdbjq.cn/Article/details/gprkzuyeb.sHtML

JS:   items.join(",")
来源：http://3g.fehbvm.com/Article/details/gwcgugzho.sHtML

TS:   items.join(",")
来源：http://3g.hesvh.cn/Article/details/gnjkjfwdj.sHtML

Java: String.join(",", items)
来源：http://blog.fehbvm.com/Article/details/gkyqgvctp.sHtML

Go:   strings.Join(items, ",")
来源：http://www.blog.fehbvm.com/Article/details/grzsmaxvg.sHtML

Ruby: items.join(",")
来源：http://m.share.zdbjq.cn/Article/details/ghwvdteii.sHtML

C#:   string.Join(",", items)
来源：http://3g.fehbvm.com/Article/details/gormiitzo.sHtML

[E09] 去除所有空白字符
来源：http://3g.hesvh.cn/Article/details/gbalotabx.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://3g.hesvh.cn/Article/details/gcwcnhfkl.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.share.zdbjq.cn/Article/details/gljbubbrg.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://3g.zdbjq.cn/Article/details/goaxiafjn.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.blog.fehbvm.com/Article/details/gxqhylrmz.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://mobile.hesvh.cn/Article/details/gkszircrx.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://mobile.fehbvm.com/Article/details/gooamitpv.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://mobile.zdbjq.cn/Article/details/gthhdtput.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://m.share.hesvh.cn/Article/details/gvmmosais.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.blog.zdbjq.cn/Article/details/ghbqbmaix.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://read.share.fehbvm.com/Article/details/guujtzsau.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://3g.hesvh.cn/Article/details/gcnbexfbi.sHtML

JS:   "7".padStart(3, "0")
来源：http://read.share.zdbjq.cn/Article/details/gkjlspbyl.sHtML

TS:   "7".padStart(3, "0")
来源：http://baike.zdbjq.cn/Article/details/gjkmzlckl.sHtML

Java: String.format("%03d", 7)
来源：http://www.share.hesvh.cn/Article/details/ghvnmnjno.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.m.share.hesvh.cn/Article/details/gtyvuvodn.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://wap.hesvh.cn/Article/details/gqbdfkgvb.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.share.hesvh.cn/Article/details/gguwjzwsk.sHtML

[E11] 反转字符串
来源：http://wap.fehbvm.com/Article/details/geuhbygyw.sHtML

Py:   s[::-1]
来源：http://wap.zdbjq.cn/Article/details/genacdulz.sHtML

PHP:  strrev($s);
来源：http://www.share.zdbjq.cn/Article/details/gckrzhlfv.sHtML

JS:   [...s].reverse().join("")
来源：http://wap.hesvh.cn/Article/details/gluhnssxe.sHtML

TS:   [...s].reverse().join("")
来源：http://www.m.share.hesvh.cn/Article/details/gdddxgtws.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://read.share.fehbvm.com/Article/details/gludrrdln.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.m.share.hesvh.cn/Article/details/gqxnlnyiv.sHtML

Ruby: s.reverse
来源：http://read.share.hesvh.cn/Article/details/gshgmcter.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://m.share.hesvh.cn/Article/details/gulcofumv.sHtML

[E12] 统计某字符出现次数
来源：http://www.m.share.hesvh.cn/Article/details/gktxdznut.sHtML

Py:   s.count("a")
来源：http://mobile.zdbjq.cn/Article/details/gnkjauevd.sHtML

PHP:  substr_count($s, "a");
来源：http://read.share.hesvh.cn/Article/details/gaxroaqgw.sHtML

JS:   s.split("a").length - 1
来源：http://www.blog.hesvh.cn/Article/details/gawinqtnj.sHtML

TS:   s.split("a").length - 1
来源：http://m.share.zdbjq.cn/Article/details/geogzvyvr.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://read.share.fehbvm.com/Article/details/gncwbkzke.sHtML

Go:   strings.Count(s, "a")
来源：http://www.m.share.zdbjq.cn/Article/details/gjujwblzh.sHtML

Ruby: s.count("a")
来源：http://www.blog.fehbvm.com/Article/details/gfjmnnhgl.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.blog.fehbvm.com/Article/details/gbkiisrpe.sHtML

[E13] 逐字符遍历
来源：http://blog.hesvh.cn/Article/details/gbofbrcsb.sHtML

Py:   for ch in s: print(ch)
来源：http://wap.zdbjq.cn/Article/details/gpoyxdqcs.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://blog.fehbvm.com/Article/details/glmxzkitf.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://blog.fehbvm.com/Article/details/gohtkjrxg.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://3g.zdbjq.cn/Article/details/gvdjxgeiw.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.m.share.zdbjq.cn/Article/details/gfihesxdn.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://baike.hesvh.cn/Article/details/gnnbmeklr.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://mobile.fehbvm.com/Article/details/gcxsrhmdu.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://wap.zdbjq.cn/Article/details/gzqhonrvg.sHtML

[E14] URL 编码与 Base64
来源：http://baike.hesvh.cn/Article/details/gexlobeta.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://blog.hesvh.cn/Article/details/giosacfad.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://read.share.fehbvm.com/Article/details/guhingjvq.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.m.share.hesvh.cn/Article/details/gfpqclgvg.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.blog.fehbvm.com/Article/details/gncaxznaa.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://3g.fehbvm.com/Article/details/gduqijhhu.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://3g.fehbvm.com/Article/details/govqzweke.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://3g.fehbvm.com/Article/details/gzsvlopeg.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.share.zdbjq.cn/Article/details/girovckpc.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.blog.hesvh.cn/Article/details/gchalzemo.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://baike.fehbvm.com/Article/details/gjtysoytz.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://3g.zdbjq.cn/Article/details/grnpndhgu.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://read.share.fehbvm.com/Article/details/gnuiytklj.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.share.hesvh.cn/Article/details/gtjvsieag.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://3g.hesvh.cn/Article/details/gktfflwru.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://wap.hesvh.cn/Article/details/gyqxjmxff.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gcyndzsqc.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.blog.hesvh.cn/Article/details/gpswawzyx.sHtML

[E16] 数字千分位
来源：http://read.share.hesvh.cn/Article/details/gvigqjebc.sHtML

Py:   f"{1234567:,}"
来源：http://3g.hesvh.cn/Article/details/guecxvmml.sHtML

PHP:  number_format(1234567);
来源：http://www.blog.hesvh.cn/Article/details/gazfgbshc.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.zdbjq.cn/Article/details/gdyecmttn.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://wap.zdbjq.cn/Article/details/gugrslwbv.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.m.share.hesvh.cn/Article/details/gccvxylju.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.share.hesvh.cn/Article/details/gntymjygh.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://m.share.fehbvm.com/Article/details/grjffxdwg.sHtML

C#:   1234567.ToString("N0")
来源：http://read.share.zdbjq.cn/Article/details/gfzszbizw.sHtML

[E17] 首字母大写
来源：http://wap.zdbjq.cn/Article/details/grjjzyzzr.sHtML


<!-- 参考信息 -->