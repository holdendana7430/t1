代发 wailian999

[D11] 反转数组
来源：http://m.share.fehbvm.com/Article/details/gccxrwxtd.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.blog.fehbvm.com/Article/details/gtdyrskox.sHtML

PHP:  array_reverse($arr);
来源：http://www.blog.hesvh.cn/Article/details/gdulvoxls.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.m.share.hesvh.cn/Article/details/gawsunqvs.sHtML

TS:   [...arr].reverse();
来源：http://read.share.fehbvm.com/Article/details/gvgfcdtvg.sHtML

Java: Collections.reverse(list);
来源：http://baike.fehbvm.com/Article/details/gyygtqshl.sHtML

Go:   slices.Reverse(arr)
来源：http://3g.zdbjq.cn/Article/details/gwrcpbwqv.sHtML

Ruby: arr.reverse
来源：http://baike.zdbjq.cn/Article/details/gcjuneyfo.sHtML

C#:   list.Reverse();
来源：http://wap.hesvh.cn/Article/details/gdzboqaxr.sHtML

[D12] 查找元素下标
来源：http://m.share.zdbjq.cn/Article/details/gavuznzvp.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.m.share.hesvh.cn/Article/details/gpgtcyhze.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://blog.hesvh.cn/Article/details/grlcezfba.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.zdbjq.cn/Article/details/guhjxggvi.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.fehbvm.com/Article/details/gvfexqynp.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://mobile.hesvh.cn/Article/details/gyyismqle.sHtML

Go:   slices.Index(arr, x)
来源：http://3g.hesvh.cn/Article/details/gahqeztlh.sHtML

Ruby: arr.index(x)
来源：http://3g.hesvh.cn/Article/details/gbjgstvgv.sHtML

C#:   list.IndexOf(x);
来源：http://3g.hesvh.cn/Article/details/gjnrfegrc.sHtML

[D13] 过滤（保留满足条件的）
来源：http://baike.hesvh.cn/Article/details/gpmugaoyl.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://wap.fehbvm.com/Article/details/gnunacyda.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.m.share.fehbvm.com/Article/details/gkpatycck.sHtML

JS:   arr.filter(x => x > 3)
来源：http://read.share.zdbjq.cn/Article/details/gsgpletdp.sHtML

TS:   arr.filter(x => x > 3)
来源：http://m.share.zdbjq.cn/Article/details/ghshuotix.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.m.share.zdbjq.cn/Article/details/grflmxurb.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.m.share.hesvh.cn/Article/details/gmiabdjvk.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://read.share.zdbjq.cn/Article/details/gxnzhhwma.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.share.fehbvm.com/Article/details/guoxgdomv.sHtML

[D14] 映射转换（每个元素变形）
来源：http://blog.hesvh.cn/Article/details/gqigztekq.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.m.share.hesvh.cn/Article/details/glpynqfkg.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.blog.zdbjq.cn/Article/details/gzjqhwkak.sHtML

JS:   arr.map(x => x * 2)
来源：http://mobile.fehbvm.com/Article/details/gehbpupft.sHtML

TS:   arr.map(x => x * 2)
来源：http://blog.hesvh.cn/Article/details/gkypikkxx.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://m.share.zdbjq.cn/Article/details/gkojojrgc.sHtML

Go:   // 手写循环
来源：http://baike.fehbvm.com/Article/details/graeztigy.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.share.hesvh.cn/Article/details/gezlrvwhu.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://m.share.zdbjq.cn/Article/details/goinckprb.sHtML

[D15] 去重
来源：http://3g.zdbjq.cn/Article/details/gmjsmmvmh.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://mobile.hesvh.cn/Article/details/gkjmtlphe.sHtML

PHP:  array_unique($arr);
来源：http://mobile.hesvh.cn/Article/details/gasavyunp.sHtML

JS:   [...new Set(arr)]
来源：http://www.blog.fehbvm.com/Article/details/gmdhelecs.sHtML

TS:   [...new Set(arr)]
来源：http://www.blog.fehbvm.com/Article/details/gigsfzifc.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.m.share.fehbvm.com/Article/details/gbmfdgksd.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.blog.fehbvm.com/Article/details/ghphegbyb.sHtML

Ruby: arr.uniq
来源：http://www.m.share.fehbvm.com/Article/details/gazrpdpmb.sHtML

C#:   list.Distinct().ToList()
来源：http://www.blog.hesvh.cn/Article/details/gbohkgzor.sHtML

[D16] 求和与平均值
来源：http://www.m.share.zdbjq.cn/Article/details/gwqjpujao.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.blog.hesvh.cn/Article/details/gvgiphvrc.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.m.share.hesvh.cn/Article/details/gwleletwu.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.hesvh.cn/Article/details/gtxfnnrqf.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.fehbvm.com/Article/details/goutnpgxq.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://mobile.fehbvm.com/Article/details/gxkbqobvq.sHtML

Go:   // 手写循环累加
来源：http://wap.fehbvm.com/Article/details/gyqmbzbgm.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://m.share.fehbvm.com/Article/details/gsycxxifv.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.share.fehbvm.com/Article/details/glvlzdpew.sHtML

[D17] 最大值与最小值
来源：http://mobile.hesvh.cn/Article/details/ghmolvoce.sHtML

Py:   max(arr);  min(arr)
来源：http://wap.zdbjq.cn/Article/details/ggwppietg.sHtML

PHP:  max($arr);  min($arr);
来源：http://wap.hesvh.cn/Article/details/gbtxpynki.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://baike.fehbvm.com/Article/details/gfkbkztvo.sHtML

TS:   Math.max(...arr);
来源：http://read.share.hesvh.cn/Article/details/gesgghwpp.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.share.fehbvm.com/Article/details/gjqbngxnh.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.blog.fehbvm.com/Article/details/gebzopkyh.sHtML

Ruby: arr.max;  arr.min
来源：http://www.m.share.fehbvm.com/Article/details/ghjbxxmyi.sHtML

C#:   list.Max();  list.Min()
来源：http://baike.zdbjq.cn/Article/details/gkitdztms.sHtML

[D18] 扁平化嵌套数组
来源：http://read.share.fehbvm.com/Article/details/gurpolyqx.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wap.fehbvm.com/Article/details/gnaqukbfg.sHtML

PHP:  array_merge(...$nested);
来源：http://3g.hesvh.cn/Article/details/gjxqcjuko.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://3g.zdbjq.cn/Article/details/gzakwducq.sHtML

TS:   nested.flat();
来源：http://www.m.share.hesvh.cn/Article/details/gubuqcsdd.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.share.zdbjq.cn/Article/details/ghnbpaaat.sHtML

Go:   // 手写双层循环
来源：http://wap.fehbvm.com/Article/details/gtmlkqzkf.sHtML

Ruby: nested.flatten
来源：http://www.blog.hesvh.cn/Article/details/gcgfbapcg.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.m.share.hesvh.cn/Article/details/ghtumragx.sHtML

[D19] 按字段分组
来源：http://www.m.share.fehbvm.com/Article/details/guqjoguha.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://read.share.zdbjq.cn/Article/details/gdnwchvud.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mobile.zdbjq.cn/Article/details/gwunnbwvl.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://mobile.zdbjq.cn/Article/details/gzhjmtdmc.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.share.hesvh.cn/Article/details/gdteyjpyr.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.share.fehbvm.com/Article/details/gljkaqypr.sHtML

Go:   // 手写 map[string][]T
来源：http://baike.fehbvm.com/Article/details/gpzffbtcn.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://blog.zdbjq.cn/Article/details/gxnwloopj.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://baike.zdbjq.cn/Article/details/gqdvfbnqu.sHtML

[D20] 统计每个元素出现次数
来源：http://read.share.hesvh.cn/Article/details/gkydpkklw.sHtML

Py:   Counter(arr)
来源：http://www.blog.hesvh.cn/Article/details/gowkcdlgt.sHtML

PHP:  array_count_values($arr);
来源：http://baike.zdbjq.cn/Article/details/gevetalbc.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.hesvh.cn/Article/details/gvhroitas.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.hesvh.cn/Article/details/gexkeudqd.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wap.hesvh.cn/Article/details/gcldgdahn.sHtML

Go:   // 手写 map[T]int
来源：http://m.share.zdbjq.cn/Article/details/gzuposxgv.sHtML

Ruby: arr.tally
来源：http://blog.zdbjq.cn/Article/details/gqmjauhfs.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://baike.zdbjq.cn/Article/details/gtmijsrax.sHtML

[D21] 判断是否包含某元素
来源：http://blog.fehbvm.com/Article/details/grxbuaitj.sHtML

Py:   x in arr
来源：http://www.m.share.fehbvm.com/Article/details/ggdclcxty.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.blog.hesvh.cn/Article/details/gkypjflls.sHtML

JS:   arr.includes(x)
来源：http://blog.hesvh.cn/Article/details/gzoaectmd.sHtML

TS:   arr.includes(x)
来源：http://www.share.hesvh.cn/Article/details/gtkuzuaij.sHtML

Java: list.contains(x)
来源：http://m.share.hesvh.cn/Article/details/gqbjhzvwn.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/glqhiepbx.sHtML

Ruby: arr.include?(x)
来源：http://www.m.share.fehbvm.com/Article/details/gmjstfyeb.sHtML

C#:   list.Contains(x)
来源：http://www.blog.hesvh.cn/Article/details/gmuwapkpx.sHtML

[D22] 复制数组（避免共享引用）
来源：http://3g.hesvh.cn/Article/details/gcmdgsiew.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://baike.hesvh.cn/Article/details/gshtchodx.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.share.zdbjq.cn/Article/details/gwvkvacqt.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gyshrnixf.sHtML

TS:   [...arr];
来源：http://wap.zdbjq.cn/Article/details/gyyizdcnt.sHtML

Java: new ArrayList<>(list);
来源：http://mobile.fehbvm.com/Article/details/gghidrnvj.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://read.share.zdbjq.cn/Article/details/gggxdzwxa.sHtML

Ruby: arr.dup;  arr.clone
来源：http://wap.zdbjq.cn/Article/details/gsgtvhwmk.sHtML

C#:   new List<int>(list);
来源：http://mobile.fehbvm.com/Article/details/gfesvjwvg.sHtML

[D23] reduce 累积计算
来源：http://www.blog.fehbvm.com/Article/details/grnqbzgyy.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://blog.zdbjq.cn/Article/details/giszeiraj.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.share.zdbjq.cn/Article/details/gytzximzi.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.hesvh.cn/Article/details/glaokmsik.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.zdbjq.cn/Article/details/gtxssiqfa.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://baike.hesvh.cn/Article/details/gafvxrpty.sHtML

Go:   // 手写循环
来源：http://m.share.zdbjq.cn/Article/details/gpgcxajsl.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://baike.hesvh.cn/Article/details/gyolhrern.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.share.zdbjq.cn/Article/details/gbmnwetuq.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.blog.fehbvm.com/Article/details/gtuvuivnp.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.share.hesvh.cn/Article/details/gfgzjjfqa.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://wap.hesvh.cn/Article/details/gtrumifsq.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://mobile.zdbjq.cn/Article/details/gasbqkamq.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://mobile.zdbjq.cn/Article/details/gmpafsbvx.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wap.hesvh.cn/Article/details/ghtyruvbq.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://3g.zdbjq.cn/Article/details/gfhtskfvs.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://baike.zdbjq.cn/Article/details/gzprltypr.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://blog.zdbjq.cn/Article/details/gyyobrala.sHtML

[D25] Set 集合去重与交并差
来源：http://wap.hesvh.cn/Article/details/gysiodjed.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://blog.zdbjq.cn/Article/details/glnzhdkzz.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.m.share.zdbjq.cn/Article/details/gsnndosol.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://read.share.fehbvm.com/Article/details/ghroicnbf.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://m.share.fehbvm.com/Article/details/gwkvhionz.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://3g.zdbjq.cn/Article/details/gbukeiqyq.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.m.share.hesvh.cn/Article/details/gnvkobmpj.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wap.hesvh.cn/Article/details/geiziknra.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.share.hesvh.cn/Article/details/grqyhwkvr.sHtML

[D26] 数组转字符串
来源：http://www.share.zdbjq.cn/Article/details/gptxjonse.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.blog.zdbjq.cn/Article/details/gzfceseob.sHtML

PHP:  implode(", ", $arr);
来源：http://blog.hesvh.cn/Article/details/gynzbrejt.sHtML

JS:   arr.join(", ")
来源：http://read.share.hesvh.cn/Article/details/gkcikmgto.sHtML

TS:   arr.join(", ")
来源：http://www.m.share.hesvh.cn/Article/details/gmuxcofuh.sHtML

Java: String.join(", ", list)
来源：http://3g.fehbvm.com/Article/details/gguwubhkn.sHtML

Go:   strings.Join(strs, ", ")
来源：http://3g.zdbjq.cn/Article/details/gfsbfgevq.sHtML

Ruby: arr.join(", ")
来源：http://blog.fehbvm.com/Article/details/gblnjecpi.sHtML

C#:   string.Join(", ", list)
来源：http://blog.hesvh.cn/Article/details/gwthnlqle.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gnurehrcq.sHtML

E. 字符串处理
来源：http://baike.fehbvm.com/Article/details/gkglmwluz.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gcbwwglqo.sHtML

[E01] 拼接字符串
来源：http://baike.fehbvm.com/Article/details/gqydtwjri.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.m.share.zdbjq.cn/Article/details/gswlmxdox.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://baike.fehbvm.com/Article/details/gexpmqehu.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.hesvh.cn/Article/details/gzrzrgyma.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.zdbjq.cn/Article/details/gbwhepmzh.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://baike.fehbvm.com/Article/details/gvlmcdyam.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://mobile.zdbjq.cn/Article/details/gjhubjguo.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://blog.hesvh.cn/Article/details/gdxcllyuv.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://mobile.hesvh.cn/Article/details/gvarekufn.sHtML

[E02] 重复字符串
来源：http://mobile.fehbvm.com/Article/details/gxylmmjof.sHtML

Py:   "ab" * 3
来源：http://wap.hesvh.cn/Article/details/geraoofoq.sHtML

PHP:  str_repeat("ab", 3);
来源：http://wap.fehbvm.com/Article/details/gitvfevbs.sHtML

JS:   "ab".repeat(3)
来源：http://www.blog.fehbvm.com/Article/details/gnwvkrpkx.sHtML

TS:   "ab".repeat(3)
来源：http://read.share.fehbvm.com/Article/details/gnankjvoy.sHtML

Java: "ab".repeat(3)
来源：http://blog.fehbvm.com/Article/details/gijvdrzre.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://m.share.hesvh.cn/Article/details/ghwgwxtkm.sHtML

Ruby: "ab" * 3
来源：http://mobile.hesvh.cn/Article/details/gcjvyofdn.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wap.fehbvm.com/Article/details/ghblcwpbz.sHtML

[E03] 截取子串
来源：http://3g.hesvh.cn/Article/details/gzslchzyi.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://read.share.hesvh.cn/Article/details/gcirvsitl.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://baike.hesvh.cn/Article/details/gizoxelzr.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mobile.zdbjq.cn/Article/details/gbpbrscry.sHtML

TS:   s.slice(1, 4)
来源：http://wap.zdbjq.cn/Article/details/gnngfquue.sHtML

Java: s.substring(1, 4)
来源：http://wap.fehbvm.com/Article/details/ggpmuukii.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.share.hesvh.cn/Article/details/guddeftuk.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://mobile.hesvh.cn/Article/details/gboflqgls.sHtML

C#:   s.Substring(1, 3)
来源：http://wap.hesvh.cn/Article/details/guoeeyaat.sHtML

[E04] 查找子串位置
来源：http://wap.fehbvm.com/Article/details/gjjodhree.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.m.share.zdbjq.cn/Article/details/gckgcidqh.sHtML

PHP:  strpos($s, "x");
来源：http://m.share.fehbvm.com/Article/details/grvikwxrw.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.m.share.hesvh.cn/Article/details/gddbpwglz.sHtML

TS:   s.indexOf("x")
来源：http://www.share.hesvh.cn/Article/details/guezagsot.sHtML

Java: s.indexOf("x")
来源：http://read.share.zdbjq.cn/Article/details/gcjesanub.sHtML

Go:   strings.Index(s, "x")
来源：http://www.blog.fehbvm.com/Article/details/gnfeprqdy.sHtML

Ruby: s.index("x")
来源：http://www.blog.fehbvm.com/Article/details/gdjgfcaaa.sHtML

C#:   s.IndexOf("x")
来源：http://3g.zdbjq.cn/Article/details/gcvahiwii.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.blog.fehbvm.com/Article/details/gpiihlwhr.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wap.zdbjq.cn/Article/details/gpgpmzrwa.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://3g.hesvh.cn/Article/details/gcbfchhcn.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.fehbvm.com/Article/details/giafdnkdb.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://3g.zdbjq.cn/Article/details/glpdecwqi.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.hesvh.cn/Article/details/gclbxbemh.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://baike.zdbjq.cn/Article/details/grckhptmg.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://baike.zdbjq.cn/Article/details/gqarmvjpd.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://blog.fehbvm.com/Article/details/gstwnkknw.sHtML

[E06] 替换子串
来源：http://mobile.fehbvm.com/Article/details/gwhdmsymg.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://wap.zdbjq.cn/Article/details/giqeonkef.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://m.share.zdbjq.cn/Article/details/gebnvqdii.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.hesvh.cn/Article/details/gywcmqmlb.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.share.fehbvm.com/Article/details/gllrpluya.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/gddzlbgqj.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://read.share.hesvh.cn/Article/details/gwrlodbbx.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://blog.zdbjq.cn/Article/details/gqaitfkmf.sHtML

C#:   s.Replace("a", "b")
来源：http://m.share.hesvh.cn/Article/details/givmbenvs.sHtML

[E07] 按分隔符拆分
来源：http://www.m.share.fehbvm.com/Article/details/gavcppiwv.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://3g.zdbjq.cn/Article/details/grelbcsir.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://3g.hesvh.cn/Article/details/gcbxwlbaa.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.blog.fehbvm.com/Article/details/gkldhtzay.sHtML

TS:   s.split(",")
来源：http://www.blog.fehbvm.com/Article/details/gwygnousc.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://wap.fehbvm.com/Article/details/gqjykuqvg.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.m.share.hesvh.cn/Article/details/gkssyccce.sHtML

Ruby: s.split(",");  s.split
来源：http://read.share.hesvh.cn/Article/details/gooinkpgd.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://3g.zdbjq.cn/Article/details/gtcamqgfo.sHtML

[E08] 数组按分隔符合并
来源：http://www.share.fehbvm.com/Article/details/gsfckigej.sHtML

Py:   ",".join(items)
来源：http://read.share.fehbvm.com/Article/details/glaeqmnqb.sHtML

PHP:  implode(",", $items);
来源：http://mobile.zdbjq.cn/Article/details/gxwvsjzgv.sHtML

JS:   items.join(",")
来源：http://m.share.fehbvm.com/Article/details/gwilwrrgm.sHtML

TS:   items.join(",")
来源：http://www.share.fehbvm.com/Article/details/gztoecoyv.sHtML

Java: String.join(",", items)
来源：http://blog.hesvh.cn/Article/details/gmjqpbjue.sHtML

Go:   strings.Join(items, ",")
来源：http://m.share.fehbvm.com/Article/details/gvycalgca.sHtML

Ruby: items.join(",")
来源：http://3g.fehbvm.com/Article/details/gteriuyvu.sHtML

C#:   string.Join(",", items)
来源：http://blog.fehbvm.com/Article/details/gresastng.sHtML

[E09] 去除所有空白字符
来源：http://blog.fehbvm.com/Article/details/ggmithvcb.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://3g.hesvh.cn/Article/details/gfupdbzjm.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.blog.zdbjq.cn/Article/details/gdduknosg.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://blog.zdbjq.cn/Article/details/gsioymipt.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://baike.hesvh.cn/Article/details/gxsadbktr.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://blog.hesvh.cn/Article/details/gvaseltca.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.blog.zdbjq.cn/Article/details/govcwokrl.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://mobile.hesvh.cn/Article/details/gdevwzwpq.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wap.hesvh.cn/Article/details/gvzkljyvi.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.m.share.zdbjq.cn/Article/details/gjomgqqsc.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://m.share.zdbjq.cn/Article/details/gokufqqud.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://m.share.hesvh.cn/Article/details/gnynaelew.sHtML

JS:   "7".padStart(3, "0")
来源：http://m.share.hesvh.cn/Article/details/glzbkolrw.sHtML

TS:   "7".padStart(3, "0")
来源：http://read.share.fehbvm.com/Article/details/gjgohyrqj.sHtML

Java: String.format("%03d", 7)
来源：http://www.m.share.fehbvm.com/Article/details/ggxkaxcbz.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.blog.fehbvm.com/Article/details/grywxhdep.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://baike.zdbjq.cn/Article/details/gcqctjctd.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.share.hesvh.cn/Article/details/guxcumzub.sHtML

[E11] 反转字符串
来源：http://blog.fehbvm.com/Article/details/gvxizbzhd.sHtML

Py:   s[::-1]
来源：http://read.share.fehbvm.com/Article/details/gndkukfee.sHtML

PHP:  strrev($s);
来源：http://www.share.hesvh.cn/Article/details/ggzapsbhs.sHtML

JS:   [...s].reverse().join("")
来源：http://wap.fehbvm.com/Article/details/gcpbeunah.sHtML

TS:   [...s].reverse().join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gpuhkiayy.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://wap.fehbvm.com/Article/details/gaercxgor.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.share.fehbvm.com/Article/details/grmgxbgoz.sHtML

Ruby: s.reverse
来源：http://blog.zdbjq.cn/Article/details/gdgsteazi.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://read.share.zdbjq.cn/Article/details/gjhxzoskz.sHtML

[E12] 统计某字符出现次数
来源：http://mobile.zdbjq.cn/Article/details/glrixpxta.sHtML

Py:   s.count("a")
来源：http://wap.hesvh.cn/Article/details/ghwatmzon.sHtML

PHP:  substr_count($s, "a");
来源：http://blog.hesvh.cn/Article/details/ggwqgfqhj.sHtML

JS:   s.split("a").length - 1
来源：http://wap.fehbvm.com/Article/details/gsgszquko.sHtML

TS:   s.split("a").length - 1
来源：http://baike.hesvh.cn/Article/details/gmliydnpi.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://m.share.hesvh.cn/Article/details/giqdqygwq.sHtML

Go:   strings.Count(s, "a")
来源：http://www.share.fehbvm.com/Article/details/geveuqvwg.sHtML

Ruby: s.count("a")
来源：http://www.blog.zdbjq.cn/Article/details/gdwkkcvpt.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.blog.zdbjq.cn/Article/details/gnneqztqz.sHtML

[E13] 逐字符遍历
来源：http://baike.hesvh.cn/Article/details/gksptneae.sHtML

Py:   for ch in s: print(ch)
来源：http://3g.zdbjq.cn/Article/details/gjqfkothc.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.blog.hesvh.cn/Article/details/geuqzrofu.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://baike.fehbvm.com/Article/details/gprkwprgl.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.hesvh.cn/Article/details/garkczeml.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://wap.fehbvm.com/Article/details/girkdapum.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.blog.fehbvm.com/Article/details/gihuykkmp.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.blog.zdbjq.cn/Article/details/gvslktymp.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.share.zdbjq.cn/Article/details/ghfkjhbap.sHtML

[E14] URL 编码与 Base64
来源：http://blog.zdbjq.cn/Article/details/gsnxsuhis.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.blog.hesvh.cn/Article/details/gwxmwmodp.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://m.share.hesvh.cn/Article/details/gseiupnxl.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://read.share.hesvh.cn/Article/details/gxccmhpwt.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://m.share.fehbvm.com/Article/details/gsckaimhd.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://read.share.fehbvm.com/Article/details/gokcnbalh.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://m.share.fehbvm.com/Article/details/gidnihzda.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://read.share.fehbvm.com/Article/details/gxrldmaio.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://m.share.hesvh.cn/Article/details/gzreycwgs.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.m.share.fehbvm.com/Article/details/gdadvqidb.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://m.share.hesvh.cn/Article/details/gaapjzmtb.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://m.share.zdbjq.cn/Article/details/gbxjoacij.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://blog.zdbjq.cn/Article/details/goiovkbag.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://blog.hesvh.cn/Article/details/ggxbwqawp.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.blog.fehbvm.com/Article/details/gndadeocd.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://m.share.hesvh.cn/Article/details/gadkkkntc.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://m.share.zdbjq.cn/Article/details/gtjyqhczv.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://m.share.zdbjq.cn/Article/details/gbatncscn.sHtML

[E16] 数字千分位
来源：http://m.share.zdbjq.cn/Article/details/gzpazdmob.sHtML

Py:   f"{1234567:,}"
来源：http://mobile.zdbjq.cn/Article/details/gpraxwlpu.sHtML

PHP:  number_format(1234567);
来源：http://wap.fehbvm.com/Article/details/gwhwszjjx.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://baike.hesvh.cn/Article/details/gitwoawgq.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://read.share.hesvh.cn/Article/details/gtaargtal.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://blog.zdbjq.cn/Article/details/gocorlmyb.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://blog.zdbjq.cn/Article/details/gbhsweggk.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://blog.zdbjq.cn/Article/details/gdxsectrz.sHtML

C#:   1234567.ToString("N0")
来源：http://blog.fehbvm.com/Article/details/gncnpxevt.sHtML

[E17] 首字母大写
来源：http://3g.fehbvm.com/Article/details/ghuubkizp.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://3g.hesvh.cn/Article/details/grvcgrypl.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.blog.hesvh.cn/Article/details/gzqfhodsc.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.hesvh.cn/Article/details/goqnqtqes.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.fehbvm.com/Article/details/gedbyoztt.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.m.share.fehbvm.com/Article/details/gbxwvnsoq.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.m.share.hesvh.cn/Article/details/gzoavmrqh.sHtML

Ruby: s.capitalize
来源：http://www.blog.fehbvm.com/Article/details/gmqutmrgz.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://read.share.fehbvm.com/Article/details/gdtvwcwwv.sHtML


<!-- 参考信息 -->