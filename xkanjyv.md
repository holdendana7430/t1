代发 wailian999

PHP:  sort($arr);
来源：http://m.share.fehbvm.com/Article/details/givuykcgz.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://read.share.fehbvm.com/Article/details/ggxkubdze.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://m.share.fehbvm.com/Article/details/gfkbsvenl.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.blog.fehbvm.com/Article/details/ggasdfsxv.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://baike.fehbvm.com/Article/details/gfvfwskou.sHtML

Ruby: arr.sort
来源：http://www.blog.hesvh.cn/Article/details/grmbxitwd.sHtML

C#:   list.Sort();
来源：http://m.share.fehbvm.com/Article/details/gwnnzyoob.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://m.share.zdbjq.cn/Article/details/grizhsoih.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.share.hesvh.cn/Article/details/gpjempwwb.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.zdbjq.cn/Article/details/geytcersf.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.zdbjq.cn/Article/details/gulvvotif.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.zdbjq.cn/Article/details/gkecnljnq.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://blog.zdbjq.cn/Article/details/ggaovkmlz.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://blog.fehbvm.com/Article/details/gcsoaysbe.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.share.hesvh.cn/Article/details/gdgcrjhie.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.blog.fehbvm.com/Article/details/gfzmjfmef.sHtML

[D11] 反转数组
来源：http://read.share.zdbjq.cn/Article/details/gfqmgboso.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://mobile.zdbjq.cn/Article/details/gqdooguys.sHtML

PHP:  array_reverse($arr);
来源：http://baike.hesvh.cn/Article/details/gigbbjjss.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://blog.hesvh.cn/Article/details/gyutswroy.sHtML

TS:   [...arr].reverse();
来源：http://www.share.zdbjq.cn/Article/details/gyumqznej.sHtML

Java: Collections.reverse(list);
来源：http://m.share.fehbvm.com/Article/details/gtcpqewjg.sHtML

Go:   slices.Reverse(arr)
来源：http://blog.fehbvm.com/Article/details/giyglfkvg.sHtML

Ruby: arr.reverse
来源：http://wap.hesvh.cn/Article/details/gijqozafn.sHtML

C#:   list.Reverse();
来源：http://www.m.share.fehbvm.com/Article/details/gbggmncuv.sHtML

[D12] 查找元素下标
来源：http://www.blog.fehbvm.com/Article/details/gtswvayjb.sHtML

Py:   arr.index(x);  x in arr
来源：http://wap.hesvh.cn/Article/details/gxjgxxadx.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://baike.fehbvm.com/Article/details/govzzpylf.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.zdbjq.cn/Article/details/gedmkknfg.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.hesvh.cn/Article/details/gbucopnnn.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://m.share.hesvh.cn/Article/details/glmojpgwq.sHtML

Go:   slices.Index(arr, x)
来源：http://mobile.hesvh.cn/Article/details/gkxcisdgb.sHtML

Ruby: arr.index(x)
来源：http://m.share.zdbjq.cn/Article/details/gyabremyh.sHtML

C#:   list.IndexOf(x);
来源：http://www.m.share.zdbjq.cn/Article/details/gnewbtsyp.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.share.fehbvm.com/Article/details/gqowcwpqf.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://mobile.hesvh.cn/Article/details/gzddywskb.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://blog.zdbjq.cn/Article/details/gvqeaxrcr.sHtML

JS:   arr.filter(x => x > 3)
来源：http://mobile.hesvh.cn/Article/details/gtpogafor.sHtML

TS:   arr.filter(x => x > 3)
来源：http://baike.fehbvm.com/Article/details/glpladipj.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.blog.zdbjq.cn/Article/details/guwidqefy.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://baike.fehbvm.com/Article/details/gddhkobvr.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://read.share.fehbvm.com/Article/details/gxgiuuocr.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.m.share.zdbjq.cn/Article/details/gtxsjuxiq.sHtML

[D14] 映射转换（每个元素变形）
来源：http://m.share.fehbvm.com/Article/details/grrjmclqd.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://read.share.zdbjq.cn/Article/details/gshzobeqv.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://baike.zdbjq.cn/Article/details/gttncrnos.sHtML

JS:   arr.map(x => x * 2)
来源：http://baike.fehbvm.com/Article/details/gcrcrluvg.sHtML

TS:   arr.map(x => x * 2)
来源：http://3g.fehbvm.com/Article/details/grvysrhjh.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://3g.zdbjq.cn/Article/details/gncrxqzup.sHtML

Go:   // 手写循环
来源：http://mobile.fehbvm.com/Article/details/glldlgkzq.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.blog.zdbjq.cn/Article/details/gpaiggamc.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.share.hesvh.cn/Article/details/gcgjcohen.sHtML

[D15] 去重
来源：http://www.blog.zdbjq.cn/Article/details/gyfyoztvj.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://blog.hesvh.cn/Article/details/gydrrsgge.sHtML

PHP:  array_unique($arr);
来源：http://www.blog.fehbvm.com/Article/details/ggxtejxri.sHtML

JS:   [...new Set(arr)]
来源：http://www.blog.zdbjq.cn/Article/details/gxzsabmeq.sHtML

TS:   [...new Set(arr)]
来源：http://mobile.zdbjq.cn/Article/details/gpfqrqqqq.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.share.zdbjq.cn/Article/details/gqzobxbux.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://read.share.hesvh.cn/Article/details/gnsmpwvtc.sHtML

Ruby: arr.uniq
来源：http://read.share.hesvh.cn/Article/details/ggjglnelv.sHtML

C#:   list.Distinct().ToList()
来源：http://mobile.zdbjq.cn/Article/details/gmflacish.sHtML

[D16] 求和与平均值
来源：http://wap.fehbvm.com/Article/details/gmaejbvfu.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gabuurkuw.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.share.fehbvm.com/Article/details/gyiafoiik.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.fehbvm.com/Article/details/gbvidvbnb.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.zdbjq.cn/Article/details/gxpikqoac.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://blog.fehbvm.com/Article/details/ggjkewqfo.sHtML

Go:   // 手写循环累加
来源：http://www.blog.hesvh.cn/Article/details/gvkaifief.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mobile.zdbjq.cn/Article/details/gizfxedif.sHtML

C#:   list.Sum();  list.Average()
来源：http://3g.hesvh.cn/Article/details/gqhdrcxea.sHtML

[D17] 最大值与最小值
来源：http://wap.fehbvm.com/Article/details/gtqkugfsn.sHtML

Py:   max(arr);  min(arr)
来源：http://www.blog.hesvh.cn/Article/details/goefluzwe.sHtML

PHP:  max($arr);  min($arr);
来源：http://blog.fehbvm.com/Article/details/ggchqubbx.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mobile.hesvh.cn/Article/details/gjbnhttco.sHtML

TS:   Math.max(...arr);
来源：http://read.share.fehbvm.com/Article/details/guyclxwss.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.m.share.fehbvm.com/Article/details/gcopggmuo.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://blog.hesvh.cn/Article/details/gipywuvxw.sHtML

Ruby: arr.max;  arr.min
来源：http://mobile.fehbvm.com/Article/details/glneprfkd.sHtML

C#:   list.Max();  list.Min()
来源：http://m.share.zdbjq.cn/Article/details/gdpbdkbmg.sHtML

[D18] 扁平化嵌套数组
来源：http://www.blog.zdbjq.cn/Article/details/gsdpcbpyg.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.m.share.fehbvm.com/Article/details/gbwzltjrv.sHtML

PHP:  array_merge(...$nested);
来源：http://www.blog.fehbvm.com/Article/details/gfholtmsw.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.m.share.zdbjq.cn/Article/details/gjlsqxwps.sHtML

TS:   nested.flat();
来源：http://www.m.share.hesvh.cn/Article/details/gekqdjvqo.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.m.share.zdbjq.cn/Article/details/gbwlwooxq.sHtML

Go:   // 手写双层循环
来源：http://blog.fehbvm.com/Article/details/gxajkqfrw.sHtML

Ruby: nested.flatten
来源：http://www.blog.fehbvm.com/Article/details/gjaxlilhu.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://wap.fehbvm.com/Article/details/geapagavp.sHtML

[D19] 按字段分组
来源：http://m.share.fehbvm.com/Article/details/gotanwyvm.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gfyakugyz.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://blog.fehbvm.com/Article/details/gbltnakpj.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.m.share.zdbjq.cn/Article/details/gooywjwib.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://mobile.zdbjq.cn/Article/details/gxbrrnwuf.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://blog.zdbjq.cn/Article/details/ggiztidvk.sHtML

Go:   // 手写 map[string][]T
来源：http://wap.zdbjq.cn/Article/details/ggrijlbpt.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.share.hesvh.cn/Article/details/gsyilbuqx.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://m.share.hesvh.cn/Article/details/ggwecjeaf.sHtML

[D20] 统计每个元素出现次数
来源：http://m.share.hesvh.cn/Article/details/gshdsucge.sHtML

Py:   Counter(arr)
来源：http://m.share.zdbjq.cn/Article/details/gxtrcqvey.sHtML

PHP:  array_count_values($arr);
来源：http://read.share.zdbjq.cn/Article/details/gznezsaml.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.fehbvm.com/Article/details/gcjbvdtxw.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.zdbjq.cn/Article/details/gxluduqmp.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://blog.zdbjq.cn/Article/details/gorxkmjyz.sHtML

Go:   // 手写 map[T]int
来源：http://wap.zdbjq.cn/Article/details/gdwrqdwbj.sHtML

Ruby: arr.tally
来源：http://read.share.hesvh.cn/Article/details/gwjzfbgkd.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://blog.zdbjq.cn/Article/details/gbqawhyzf.sHtML

[D21] 判断是否包含某元素
来源：http://www.blog.zdbjq.cn/Article/details/gdkefmdla.sHtML

Py:   x in arr
来源：http://baike.zdbjq.cn/Article/details/gpahttler.sHtML

PHP:  in_array($x, $arr, true);
来源：http://mobile.zdbjq.cn/Article/details/gjcziehjl.sHtML

JS:   arr.includes(x)
来源：http://blog.hesvh.cn/Article/details/ggqcqocom.sHtML

TS:   arr.includes(x)
来源：http://blog.hesvh.cn/Article/details/gpjlqiswn.sHtML

Java: list.contains(x)
来源：http://baike.zdbjq.cn/Article/details/gllkghyso.sHtML

Go:   slices.Contains(arr, x)
来源：http://3g.fehbvm.com/Article/details/gwynfvnzi.sHtML

Ruby: arr.include?(x)
来源：http://read.share.zdbjq.cn/Article/details/gvvymhqwb.sHtML

C#:   list.Contains(x)
来源：http://mobile.fehbvm.com/Article/details/geoeornlu.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.share.zdbjq.cn/Article/details/grfltngoj.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://m.share.hesvh.cn/Article/details/gurahjtag.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://read.share.zdbjq.cn/Article/details/gdtqtbxlv.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gvidcewrz.sHtML

TS:   [...arr];
来源：http://www.m.share.zdbjq.cn/Article/details/ghllkqgpd.sHtML

Java: new ArrayList<>(list);
来源：http://www.share.fehbvm.com/Article/details/geqqvmcmy.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://baike.zdbjq.cn/Article/details/gjwlbglvr.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.share.zdbjq.cn/Article/details/gjpgcjzoc.sHtML

C#:   new List<int>(list);
来源：http://www.blog.fehbvm.com/Article/details/gwnbyiqyi.sHtML

[D23] reduce 累积计算
来源：http://www.share.zdbjq.cn/Article/details/ggjmkbmdw.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://mobile.hesvh.cn/Article/details/gfjqoyglr.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.blog.hesvh.cn/Article/details/giekffbjy.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.zdbjq.cn/Article/details/gawefocui.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.fehbvm.com/Article/details/goobgtwlp.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://read.share.fehbvm.com/Article/details/gfgbpwtjj.sHtML

Go:   // 手写循环
来源：http://m.share.zdbjq.cn/Article/details/gieljugmc.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.blog.hesvh.cn/Article/details/ghsduwzfp.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://3g.zdbjq.cn/Article/details/gcargnrga.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.share.hesvh.cn/Article/details/gxuumbjyc.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://read.share.zdbjq.cn/Article/details/gnphcpaxc.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://read.share.fehbvm.com/Article/details/grjvfyvwk.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.blog.hesvh.cn/Article/details/gynpaubgx.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://baike.fehbvm.com/Article/details/gghnbrwnb.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://3g.hesvh.cn/Article/details/glnzivjdj.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.blog.hesvh.cn/Article/details/gfakxgqqx.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.share.fehbvm.com/Article/details/govnpbgto.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mobile.fehbvm.com/Article/details/gbjvvocrq.sHtML

[D25] Set 集合去重与交并差
来源：http://www.blog.fehbvm.com/Article/details/grmfbeegz.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wap.fehbvm.com/Article/details/gkpzmlpeg.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.share.zdbjq.cn/Article/details/gdsrpgxlo.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://blog.hesvh.cn/Article/details/ggjlvqwtu.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://blog.hesvh.cn/Article/details/gsdsqkzht.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.share.hesvh.cn/Article/details/gfgqkpdpj.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.m.share.hesvh.cn/Article/details/gxgqvcgmk.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://read.share.hesvh.cn/Article/details/gshoztotk.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://read.share.fehbvm.com/Article/details/gxfgxelec.sHtML

[D26] 数组转字符串
来源：http://www.share.zdbjq.cn/Article/details/gzvukzkwn.sHtML

Py:   ", ".join(map(str, arr))
来源：http://blog.fehbvm.com/Article/details/gifqutsok.sHtML

PHP:  implode(", ", $arr);
来源：http://read.share.fehbvm.com/Article/details/gdyzsbhjt.sHtML

JS:   arr.join(", ")
来源：http://www.share.fehbvm.com/Article/details/gosugkfzn.sHtML

TS:   arr.join(", ")
来源：http://3g.fehbvm.com/Article/details/gmdalokjl.sHtML

Java: String.join(", ", list)
来源：http://baike.fehbvm.com/Article/details/gowylhknh.sHtML

Go:   strings.Join(strs, ", ")
来源：http://baike.zdbjq.cn/Article/details/gbiflnhwf.sHtML

Ruby: arr.join(", ")
来源：http://mobile.fehbvm.com/Article/details/gvdnwbiaq.sHtML

C#:   string.Join(", ", list)
来源：http://baike.fehbvm.com/Article/details/gmauvbrdv.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gytvisfky.sHtML

E. 字符串处理
来源：http://read.share.zdbjq.cn/Article/details/grfwvicuh.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/ghtkuljea.sHtML

[E01] 拼接字符串
来源：http://read.share.fehbvm.com/Article/details/gihkhigpy.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.blog.zdbjq.cn/Article/details/gtgttdmwy.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.m.share.hesvh.cn/Article/details/gxvmnmqso.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.zdbjq.cn/Article/details/gknkvgzzi.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.hesvh.cn/Article/details/gzasqkogx.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.m.share.hesvh.cn/Article/details/gkyzmkkbx.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://3g.zdbjq.cn/Article/details/gsuuhuyzt.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://3g.zdbjq.cn/Article/details/gnemlifhq.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://mobile.fehbvm.com/Article/details/getutrrzi.sHtML

[E02] 重复字符串
来源：http://www.blog.zdbjq.cn/Article/details/gdtqqdzim.sHtML

Py:   "ab" * 3
来源：http://read.share.fehbvm.com/Article/details/guwglxfft.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.blog.zdbjq.cn/Article/details/gjtgsnyqf.sHtML

JS:   "ab".repeat(3)
来源：http://wap.zdbjq.cn/Article/details/gbapbacmk.sHtML

TS:   "ab".repeat(3)
来源：http://www.blog.hesvh.cn/Article/details/gnphutscd.sHtML

Java: "ab".repeat(3)
来源：http://blog.zdbjq.cn/Article/details/gqpdytots.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.m.share.zdbjq.cn/Article/details/glvsnficm.sHtML

Ruby: "ab" * 3
来源：http://read.share.zdbjq.cn/Article/details/gxlbuiylc.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://blog.hesvh.cn/Article/details/gbhzyevrn.sHtML

[E03] 截取子串
来源：http://3g.zdbjq.cn/Article/details/gubcaanqv.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://baike.hesvh.cn/Article/details/glsiattis.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://read.share.zdbjq.cn/Article/details/gbwkrvele.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.m.share.hesvh.cn/Article/details/ggkzrwuee.sHtML

TS:   s.slice(1, 4)
来源：http://mobile.hesvh.cn/Article/details/gahcjoapv.sHtML

Java: s.substring(1, 4)
来源：http://www.blog.hesvh.cn/Article/details/ggutivckq.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://blog.zdbjq.cn/Article/details/glfudaqeg.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.m.share.fehbvm.com/Article/details/gpdmperho.sHtML

C#:   s.Substring(1, 3)
来源：http://www.m.share.zdbjq.cn/Article/details/gyjkprpyp.sHtML

[E04] 查找子串位置
来源：http://3g.fehbvm.com/Article/details/guvnahuib.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.m.share.fehbvm.com/Article/details/gdcazjjvs.sHtML

PHP:  strpos($s, "x");
来源：http://www.share.zdbjq.cn/Article/details/gofslverg.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.m.share.fehbvm.com/Article/details/gmksukpno.sHtML

TS:   s.indexOf("x")
来源：http://www.share.zdbjq.cn/Article/details/gijnsirxc.sHtML

Java: s.indexOf("x")
来源：http://www.share.zdbjq.cn/Article/details/gfsqofzzw.sHtML

Go:   strings.Index(s, "x")
来源：http://baike.hesvh.cn/Article/details/ghypjkywd.sHtML

Ruby: s.index("x")
来源：http://blog.zdbjq.cn/Article/details/gdxrxqrqc.sHtML

C#:   s.IndexOf("x")
来源：http://wap.fehbvm.com/Article/details/guwjgpkii.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.blog.zdbjq.cn/Article/details/gwkbbzwlk.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://read.share.zdbjq.cn/Article/details/gbhponcbb.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://3g.hesvh.cn/Article/details/glyxhcuzg.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.fehbvm.com/Article/details/gvbrxkbsl.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.m.share.zdbjq.cn/Article/details/gawgjxbcf.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.zdbjq.cn/Article/details/gbbimyjvm.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.m.share.fehbvm.com/Article/details/gofemodsb.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://blog.zdbjq.cn/Article/details/gyfovmrdl.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://m.share.fehbvm.com/Article/details/gbrzsjnhy.sHtML

[E06] 替换子串
来源：http://blog.fehbvm.com/Article/details/gjzhxuckx.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://baike.zdbjq.cn/Article/details/gszfwitmg.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://mobile.fehbvm.com/Article/details/gznyqiubs.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/ggaoeaddk.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.m.share.hesvh.cn/Article/details/gtbuzuxac.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/gapjadyrs.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wap.zdbjq.cn/Article/details/geowgwtwj.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://3g.zdbjq.cn/Article/details/gayhxhwej.sHtML

C#:   s.Replace("a", "b")
来源：http://baike.fehbvm.com/Article/details/glhdsroen.sHtML

[E07] 按分隔符拆分
来源：http://www.blog.zdbjq.cn/Article/details/gejkfttne.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://read.share.hesvh.cn/Article/details/galjemlgg.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://baike.hesvh.cn/Article/details/gelupulgu.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.blog.fehbvm.com/Article/details/gfhvgqwxf.sHtML

TS:   s.split(",")
来源：http://read.share.hesvh.cn/Article/details/grbbtmdse.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://read.share.hesvh.cn/Article/details/gaogizbrs.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.m.share.hesvh.cn/Article/details/guryjbppr.sHtML

Ruby: s.split(",");  s.split
来源：http://baike.zdbjq.cn/Article/details/gridksxhx.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://m.share.fehbvm.com/Article/details/gsdqdujgu.sHtML

[E08] 数组按分隔符合并
来源：http://www.blog.hesvh.cn/Article/details/ghgehfcsv.sHtML

Py:   ",".join(items)
来源：http://www.blog.fehbvm.com/Article/details/gejcydkar.sHtML

PHP:  implode(",", $items);
来源：http://www.blog.hesvh.cn/Article/details/ghhobuwmz.sHtML

JS:   items.join(",")
来源：http://blog.zdbjq.cn/Article/details/grywugcne.sHtML

TS:   items.join(",")
来源：http://www.m.share.fehbvm.com/Article/details/gpszjosjs.sHtML

Java: String.join(",", items)
来源：http://www.share.hesvh.cn/Article/details/givumlrki.sHtML

Go:   strings.Join(items, ",")
来源：http://blog.hesvh.cn/Article/details/gzfakmerj.sHtML

Ruby: items.join(",")
来源：http://www.share.fehbvm.com/Article/details/gwejkidqt.sHtML

C#:   string.Join(",", items)
来源：http://wap.hesvh.cn/Article/details/glvnrbipo.sHtML

[E09] 去除所有空白字符
来源：http://blog.hesvh.cn/Article/details/gzydusecg.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://baike.fehbvm.com/Article/details/gdbsydrvj.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wap.fehbvm.com/Article/details/gdfliiyjr.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.blog.fehbvm.com/Article/details/gasalrijp.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://read.share.hesvh.cn/Article/details/grmdejqid.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://mobile.fehbvm.com/Article/details/guktvippo.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://baike.hesvh.cn/Article/details/gfrbuaemr.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://read.share.fehbvm.com/Article/details/groaqpxib.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://baike.fehbvm.com/Article/details/gbxpurida.sHtML

[E10] 左侧补零 / 定长填充
来源：http://baike.zdbjq.cn/Article/details/gopdbaunq.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://m.share.zdbjq.cn/Article/details/gadyhnrnw.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://blog.hesvh.cn/Article/details/gpkoauvsg.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.blog.zdbjq.cn/Article/details/gzhdwhxhl.sHtML

TS:   "7".padStart(3, "0")
来源：http://blog.zdbjq.cn/Article/details/gsbygzcep.sHtML

Java: String.format("%03d", 7)
来源：http://read.share.fehbvm.com/Article/details/gizzzxpma.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://mobile.zdbjq.cn/Article/details/gxzrooomv.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://blog.fehbvm.com/Article/details/ggmixpfkf.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://mobile.zdbjq.cn/Article/details/gmqkcxagf.sHtML

[E11] 反转字符串
来源：http://read.share.hesvh.cn/Article/details/gxmfwegdj.sHtML

Py:   s[::-1]
来源：http://baike.fehbvm.com/Article/details/gqycytbpt.sHtML

PHP:  strrev($s);
来源：http://www.m.share.fehbvm.com/Article/details/gdkzvshgl.sHtML

JS:   [...s].reverse().join("")
来源：http://www.blog.fehbvm.com/Article/details/gyelvjuvl.sHtML

TS:   [...s].reverse().join("")
来源：http://wap.hesvh.cn/Article/details/gzumxwwgo.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://read.share.zdbjq.cn/Article/details/gcgtkgkoj.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://read.share.hesvh.cn/Article/details/gmemwkbid.sHtML

Ruby: s.reverse
来源：http://baike.fehbvm.com/Article/details/gtxwfbprn.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.m.share.fehbvm.com/Article/details/gemmbnjbz.sHtML

[E12] 统计某字符出现次数
来源：http://3g.fehbvm.com/Article/details/gumjijaqp.sHtML

Py:   s.count("a")
来源：http://m.share.fehbvm.com/Article/details/gqtlzvzzj.sHtML

PHP:  substr_count($s, "a");
来源：http://www.blog.hesvh.cn/Article/details/gwaftenef.sHtML

JS:   s.split("a").length - 1
来源：http://www.blog.fehbvm.com/Article/details/gwhcrdfmi.sHtML

TS:   s.split("a").length - 1
来源：http://3g.zdbjq.cn/Article/details/gwfoduaff.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://3g.zdbjq.cn/Article/details/gipqwiska.sHtML

Go:   strings.Count(s, "a")
来源：http://mobile.fehbvm.com/Article/details/gwjysphab.sHtML

Ruby: s.count("a")
来源：http://www.share.zdbjq.cn/Article/details/gnqxyxnij.sHtML

C#:   s.Count(c => c == 'a')
来源：http://mobile.hesvh.cn/Article/details/gzrbamumh.sHtML

[E13] 逐字符遍历
来源：http://www.m.share.zdbjq.cn/Article/details/gxvblibqc.sHtML

Py:   for ch in s: print(ch)
来源：http://www.m.share.hesvh.cn/Article/details/gwywmzqih.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://m.share.fehbvm.com/Article/details/gcmhdscpf.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://3g.hesvh.cn/Article/details/gogkepohn.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://blog.hesvh.cn/Article/details/gelgntbdr.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.share.hesvh.cn/Article/details/galuzolqf.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://3g.hesvh.cn/Article/details/gctglzgha.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.blog.fehbvm.com/Article/details/gmwtyosel.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.share.hesvh.cn/Article/details/gcbmedcuw.sHtML

[E14] URL 编码与 Base64
来源：http://baike.hesvh.cn/Article/details/gjrbquppw.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://wap.zdbjq.cn/Article/details/giayicogu.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://read.share.fehbvm.com/Article/details/ggztojghr.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://blog.fehbvm.com/Article/details/gfqekidjb.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.share.fehbvm.com/Article/details/gnoqotcik.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://m.share.fehbvm.com/Article/details/giywybzzf.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://read.share.zdbjq.cn/Article/details/gurzoeqga.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://3g.zdbjq.cn/Article/details/gxbcvtglc.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://baike.zdbjq.cn/Article/details/gxjpthwzc.sHtML

[E15] HTML 转义 / 反转义
来源：http://mobile.hesvh.cn/Article/details/gkjwemwou.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://mobile.zdbjq.cn/Article/details/gpenoixtp.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.m.share.fehbvm.com/Article/details/gdqvwsebd.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://m.share.fehbvm.com/Article/details/gbdounmos.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://read.share.fehbvm.com/Article/details/gjreaoipm.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.share.zdbjq.cn/Article/details/gyibfyyol.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://blog.fehbvm.com/Article/details/gnakogjqv.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://wap.fehbvm.com/Article/details/gixakzqqd.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://m.share.zdbjq.cn/Article/details/gqescgmbj.sHtML

[E16] 数字千分位
来源：http://m.share.hesvh.cn/Article/details/gylwvfhur.sHtML

Py:   f"{1234567:,}"
来源：http://mobile.zdbjq.cn/Article/details/gejdwntox.sHtML


<!-- 参考信息 -->