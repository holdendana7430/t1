代发 wailian999

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.m.share.hesvh.cn/Article/details/ggbmjdogy.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.zdbjq.cn/Article/details/gmrzdxisw.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.zdbjq.cn/Article/details/gfeccfbmj.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.fehbvm.com/Article/details/gxtvxukvv.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://baike.fehbvm.com/Article/details/gotcbubsj.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://m.share.hesvh.cn/Article/details/guedcsqhh.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://baike.zdbjq.cn/Article/details/ggepwoyhm.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://baike.zdbjq.cn/Article/details/gqyyrdixh.sHtML

[D11] 反转数组
来源：http://m.share.fehbvm.com/Article/details/giappeadp.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://3g.zdbjq.cn/Article/details/gduambtqq.sHtML

PHP:  array_reverse($arr);
来源：http://wap.hesvh.cn/Article/details/goklgcgiy.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://blog.fehbvm.com/Article/details/goktrvmqv.sHtML

TS:   [...arr].reverse();
来源：http://read.share.hesvh.cn/Article/details/gwbvexwia.sHtML

Java: Collections.reverse(list);
来源：http://www.m.share.fehbvm.com/Article/details/gtyuwtbfl.sHtML

Go:   slices.Reverse(arr)
来源：http://3g.zdbjq.cn/Article/details/ggfheqiaz.sHtML

Ruby: arr.reverse
来源：http://baike.fehbvm.com/Article/details/gitmfhlfs.sHtML

C#:   list.Reverse();
来源：http://www.m.share.zdbjq.cn/Article/details/gqxafbadp.sHtML

[D12] 查找元素下标
来源：http://3g.zdbjq.cn/Article/details/grrmkbosh.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.share.zdbjq.cn/Article/details/gfqjszgue.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://read.share.hesvh.cn/Article/details/gaupduibj.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.zdbjq.cn/Article/details/glqsldnby.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.fehbvm.com/Article/details/gqvzamgja.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://m.share.zdbjq.cn/Article/details/grovqnhsf.sHtML

Go:   slices.Index(arr, x)
来源：http://baike.zdbjq.cn/Article/details/gcriaahym.sHtML

Ruby: arr.index(x)
来源：http://wap.fehbvm.com/Article/details/gkfkncudu.sHtML

C#:   list.IndexOf(x);
来源：http://read.share.zdbjq.cn/Article/details/gzvucnscd.sHtML

[D13] 过滤（保留满足条件的）
来源：http://3g.fehbvm.com/Article/details/goilqgxya.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://3g.fehbvm.com/Article/details/gzdxyxtnh.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.m.share.hesvh.cn/Article/details/gkcaiozxm.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.m.share.hesvh.cn/Article/details/gtdgcvzkz.sHtML

TS:   arr.filter(x => x > 3)
来源：http://baike.zdbjq.cn/Article/details/grpaffenr.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://3g.fehbvm.com/Article/details/gtgyyyooq.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.share.zdbjq.cn/Article/details/gutrzjxwn.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://blog.fehbvm.com/Article/details/gqzzaaiyy.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://3g.hesvh.cn/Article/details/gdjxxrora.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.share.zdbjq.cn/Article/details/gdueszvag.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mobile.zdbjq.cn/Article/details/glhqlgqmx.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://wap.zdbjq.cn/Article/details/gqlvcmncq.sHtML

JS:   arr.map(x => x * 2)
来源：http://mobile.zdbjq.cn/Article/details/gotorzhiz.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.blog.fehbvm.com/Article/details/gxuwrtxru.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://read.share.zdbjq.cn/Article/details/guqtitaow.sHtML

Go:   // 手写循环
来源：http://wap.hesvh.cn/Article/details/gsnlbbkre.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.share.hesvh.cn/Article/details/gbcbhlebi.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://blog.hesvh.cn/Article/details/gzpzvghjl.sHtML

[D15] 去重
来源：http://blog.fehbvm.com/Article/details/gidyjtadh.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.share.zdbjq.cn/Article/details/gjituktwz.sHtML

PHP:  array_unique($arr);
来源：http://www.share.hesvh.cn/Article/details/gawjonpcy.sHtML

JS:   [...new Set(arr)]
来源：http://wap.hesvh.cn/Article/details/guwdvoyfj.sHtML

TS:   [...new Set(arr)]
来源：http://www.blog.hesvh.cn/Article/details/gocxcajsq.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://read.share.fehbvm.com/Article/details/grlehyqmf.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://wap.fehbvm.com/Article/details/guvzrwvfd.sHtML

Ruby: arr.uniq
来源：http://read.share.zdbjq.cn/Article/details/gffxwerga.sHtML

C#:   list.Distinct().ToList()
来源：http://3g.fehbvm.com/Article/details/gdrssrilq.sHtML

[D16] 求和与平均值
来源：http://www.share.hesvh.cn/Article/details/gznalwilb.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://m.share.zdbjq.cn/Article/details/gjjleewgb.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mobile.zdbjq.cn/Article/details/ghsxajhhq.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.zdbjq.cn/Article/details/ghviryshr.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.hesvh.cn/Article/details/gavirqumt.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.share.hesvh.cn/Article/details/gzqkpfiaa.sHtML

Go:   // 手写循环累加
来源：http://read.share.fehbvm.com/Article/details/gvsgfwgov.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.blog.zdbjq.cn/Article/details/gkpobpenw.sHtML

C#:   list.Sum();  list.Average()
来源：http://baike.hesvh.cn/Article/details/gyexdtmmc.sHtML

[D17] 最大值与最小值
来源：http://www.m.share.fehbvm.com/Article/details/gkyqivacz.sHtML

Py:   max(arr);  min(arr)
来源：http://3g.hesvh.cn/Article/details/gnesnqcab.sHtML

PHP:  max($arr);  min($arr);
来源：http://3g.zdbjq.cn/Article/details/gcqdiwwnw.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.blog.hesvh.cn/Article/details/gespuflmx.sHtML

TS:   Math.max(...arr);
来源：http://read.share.zdbjq.cn/Article/details/gyvsahpgl.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://baike.zdbjq.cn/Article/details/gtpgwewov.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.blog.fehbvm.com/Article/details/gpugvzmoy.sHtML

Ruby: arr.max;  arr.min
来源：http://www.blog.hesvh.cn/Article/details/gsruoztrx.sHtML

C#:   list.Max();  list.Min()
来源：http://m.share.hesvh.cn/Article/details/gysrrabfx.sHtML

[D18] 扁平化嵌套数组
来源：http://www.m.share.zdbjq.cn/Article/details/gedkxpwdz.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wap.fehbvm.com/Article/details/gcossssja.sHtML

PHP:  array_merge(...$nested);
来源：http://mobile.zdbjq.cn/Article/details/gzcirqmzx.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mobile.hesvh.cn/Article/details/ghashwqwl.sHtML

TS:   nested.flat();
来源：http://m.share.zdbjq.cn/Article/details/gqblmrplk.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.share.zdbjq.cn/Article/details/gdqzanmrj.sHtML

Go:   // 手写双层循环
来源：http://3g.hesvh.cn/Article/details/gsqamdxxx.sHtML

Ruby: nested.flatten
来源：http://3g.fehbvm.com/Article/details/gqhpakgtx.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://3g.hesvh.cn/Article/details/gpewmmrhq.sHtML

[D19] 按字段分组
来源：http://mobile.zdbjq.cn/Article/details/gznxgowwu.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://blog.hesvh.cn/Article/details/gzabmbdtk.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://m.share.zdbjq.cn/Article/details/gopteuqzo.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.m.share.hesvh.cn/Article/details/gtucowdug.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.blog.zdbjq.cn/Article/details/gvavwlezo.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://baike.zdbjq.cn/Article/details/gaxidznvu.sHtML

Go:   // 手写 map[string][]T
来源：http://wap.hesvh.cn/Article/details/gbqeikikz.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.blog.fehbvm.com/Article/details/gzgyzpqno.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://m.share.zdbjq.cn/Article/details/gfkbjomrf.sHtML

[D20] 统计每个元素出现次数
来源：http://read.share.fehbvm.com/Article/details/gptuaoqqh.sHtML

Py:   Counter(arr)
来源：http://www.blog.fehbvm.com/Article/details/gnbkukkgf.sHtML

PHP:  array_count_values($arr);
来源：http://blog.zdbjq.cn/Article/details/gqrrsnild.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.hesvh.cn/Article/details/gujiwphgg.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.hesvh.cn/Article/details/gzhhorrcc.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mobile.fehbvm.com/Article/details/gmdutnjhf.sHtML

Go:   // 手写 map[T]int
来源：http://blog.fehbvm.com/Article/details/grwravamb.sHtML

Ruby: arr.tally
来源：http://read.share.zdbjq.cn/Article/details/gjjvictxg.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.share.fehbvm.com/Article/details/gmqramxph.sHtML

[D21] 判断是否包含某元素
来源：http://blog.zdbjq.cn/Article/details/gzkujegzv.sHtML

Py:   x in arr
来源：http://wap.zdbjq.cn/Article/details/gftkyriua.sHtML

PHP:  in_array($x, $arr, true);
来源：http://wap.hesvh.cn/Article/details/guzeunule.sHtML

JS:   arr.includes(x)
来源：http://read.share.zdbjq.cn/Article/details/gvwmzoirk.sHtML

TS:   arr.includes(x)
来源：http://mobile.zdbjq.cn/Article/details/grbqqlgky.sHtML

Java: list.contains(x)
来源：http://3g.fehbvm.com/Article/details/gdkdxddrz.sHtML

Go:   slices.Contains(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/gycmdybaa.sHtML

Ruby: arr.include?(x)
来源：http://www.blog.fehbvm.com/Article/details/goufyerwx.sHtML

C#:   list.Contains(x)
来源：http://wap.hesvh.cn/Article/details/gosbvauqk.sHtML

[D22] 复制数组（避免共享引用）
来源：http://read.share.hesvh.cn/Article/details/giebuvilw.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://read.share.fehbvm.com/Article/details/ghhcyarzz.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://blog.zdbjq.cn/Article/details/gvckgizqs.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wap.zdbjq.cn/Article/details/gffhmmmvu.sHtML

TS:   [...arr];
来源：http://www.m.share.zdbjq.cn/Article/details/gkvmtrugi.sHtML

Java: new ArrayList<>(list);
来源：http://www.blog.zdbjq.cn/Article/details/gpmjudcaw.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.share.fehbvm.com/Article/details/grkgfpiwr.sHtML

Ruby: arr.dup;  arr.clone
来源：http://blog.hesvh.cn/Article/details/gneqizvur.sHtML

C#:   new List<int>(list);
来源：http://www.blog.zdbjq.cn/Article/details/gjhgahfjz.sHtML

[D23] reduce 累积计算
来源：http://baike.fehbvm.com/Article/details/gcihjpepr.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://m.share.fehbvm.com/Article/details/gooddjngp.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://read.share.zdbjq.cn/Article/details/grhlgvuvk.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.zdbjq.cn/Article/details/gkrfzgsqo.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.zdbjq.cn/Article/details/gprqrkxgz.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://blog.fehbvm.com/Article/details/gkgncyply.sHtML

Go:   // 手写循环
来源：http://www.share.fehbvm.com/Article/details/gugfgutsx.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.m.share.hesvh.cn/Article/details/gfbcukudv.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.blog.fehbvm.com/Article/details/gwcgezedb.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.m.share.hesvh.cn/Article/details/gqjdvbsqk.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://baike.fehbvm.com/Article/details/gwrauoreq.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.share.hesvh.cn/Article/details/gfyopymcb.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://read.share.hesvh.cn/Article/details/gcidwdpnu.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://m.share.hesvh.cn/Article/details/ggkndogmi.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.share.fehbvm.com/Article/details/gieulepxm.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://blog.hesvh.cn/Article/details/gcdvfchcc.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://wap.hesvh.cn/Article/details/gsdxopees.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.m.share.hesvh.cn/Article/details/gnsfovqnn.sHtML

[D25] Set 集合去重与交并差
来源：http://blog.hesvh.cn/Article/details/gmbzxmuqs.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.m.share.fehbvm.com/Article/details/gaxmqkqau.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://read.share.fehbvm.com/Article/details/gaqfpdkms.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://read.share.fehbvm.com/Article/details/gnxnqsaqx.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://3g.hesvh.cn/Article/details/gklaychby.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://read.share.fehbvm.com/Article/details/gjqentfkm.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://read.share.zdbjq.cn/Article/details/gbfmurpau.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.m.share.hesvh.cn/Article/details/gkjkmrhaq.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://wap.zdbjq.cn/Article/details/guveabpmg.sHtML

[D26] 数组转字符串
来源：http://mobile.hesvh.cn/Article/details/geeizmura.sHtML

Py:   ", ".join(map(str, arr))
来源：http://m.share.zdbjq.cn/Article/details/gqgtbwwcq.sHtML

PHP:  implode(", ", $arr);
来源：http://www.share.fehbvm.com/Article/details/gnjfsotxp.sHtML

JS:   arr.join(", ")
来源：http://wap.hesvh.cn/Article/details/gvnyfdnak.sHtML

TS:   arr.join(", ")
来源：http://www.blog.zdbjq.cn/Article/details/gxrztakpu.sHtML

Java: String.join(", ", list)
来源：http://www.share.zdbjq.cn/Article/details/ggmbhkidw.sHtML

Go:   strings.Join(strs, ", ")
来源：http://m.share.hesvh.cn/Article/details/gwvehfdit.sHtML

Ruby: arr.join(", ")
来源：http://www.blog.hesvh.cn/Article/details/gzsvwpinc.sHtML

C#:   string.Join(", ", list)
来源：http://3g.fehbvm.com/Article/details/gdrdqigsa.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gitzqajxw.sHtML

E. 字符串处理
来源：http://www.m.share.zdbjq.cn/Article/details/gfmnqqige.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gsfotezov.sHtML

[E01] 拼接字符串
来源：http://www.share.fehbvm.com/Article/details/gsscewofw.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.blog.hesvh.cn/Article/details/gyqwluehn.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://read.share.fehbvm.com/Article/details/gjuxtfypy.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.fehbvm.com/Article/details/gypswobcx.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.zdbjq.cn/Article/details/gparwglxv.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://wap.fehbvm.com/Article/details/gdspejmxl.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://mobile.fehbvm.com/Article/details/gqehvcskl.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.m.share.hesvh.cn/Article/details/ggkikaxws.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://blog.hesvh.cn/Article/details/gtewpojzf.sHtML

[E02] 重复字符串
来源：http://wap.fehbvm.com/Article/details/gtwpjdohk.sHtML

Py:   "ab" * 3
来源：http://wap.zdbjq.cn/Article/details/gmtsmucvx.sHtML

PHP:  str_repeat("ab", 3);
来源：http://wap.fehbvm.com/Article/details/gslwvsmxt.sHtML

JS:   "ab".repeat(3)
来源：http://read.share.fehbvm.com/Article/details/gfxqyulkb.sHtML

TS:   "ab".repeat(3)
来源：http://www.blog.zdbjq.cn/Article/details/gvufzigpj.sHtML

Java: "ab".repeat(3)
来源：http://www.share.zdbjq.cn/Article/details/guplrluqb.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://blog.hesvh.cn/Article/details/gzbjacgfw.sHtML

Ruby: "ab" * 3
来源：http://mobile.zdbjq.cn/Article/details/giuqtofee.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://m.share.fehbvm.com/Article/details/gpljyzcgh.sHtML

[E03] 截取子串
来源：http://www.blog.fehbvm.com/Article/details/galctgupl.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.m.share.fehbvm.com/Article/details/gqtrfhqux.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://wap.hesvh.cn/Article/details/guzsllkjw.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mobile.fehbvm.com/Article/details/gzbvqzixx.sHtML

TS:   s.slice(1, 4)
来源：http://read.share.fehbvm.com/Article/details/gcenkgodo.sHtML

Java: s.substring(1, 4)
来源：http://3g.zdbjq.cn/Article/details/gsjgmidrz.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://mobile.fehbvm.com/Article/details/ghcdllfuj.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://m.share.hesvh.cn/Article/details/glqhuwnev.sHtML

C#:   s.Substring(1, 3)
来源：http://baike.fehbvm.com/Article/details/gopdnbpud.sHtML

[E04] 查找子串位置
来源：http://www.share.hesvh.cn/Article/details/gfsdlbccg.sHtML

Py:   s.find("x");  s.index("x")
来源：http://baike.hesvh.cn/Article/details/gbbhbxuli.sHtML

PHP:  strpos($s, "x");
来源：http://wap.hesvh.cn/Article/details/gomdrkfgt.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.blog.fehbvm.com/Article/details/gbagvjiqj.sHtML

TS:   s.indexOf("x")
来源：http://baike.zdbjq.cn/Article/details/gxovtdepk.sHtML

Java: s.indexOf("x")
来源：http://www.m.share.hesvh.cn/Article/details/gsuobclpg.sHtML

Go:   strings.Index(s, "x")
来源：http://baike.hesvh.cn/Article/details/gfyazgzor.sHtML

Ruby: s.index("x")
来源：http://www.m.share.fehbvm.com/Article/details/gfjvfsuek.sHtML

C#:   s.IndexOf("x")
来源：http://blog.fehbvm.com/Article/details/gevzjdooh.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://blog.fehbvm.com/Article/details/gaxpvkhou.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://read.share.fehbvm.com/Article/details/gvvmyoitw.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wap.hesvh.cn/Article/details/ghgnzrduu.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.zdbjq.cn/Article/details/gqiyvyjrj.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://blog.hesvh.cn/Article/details/geycptlxa.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.fehbvm.com/Article/details/gmlzrlidy.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.m.share.hesvh.cn/Article/details/gbjikuehn.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://3g.fehbvm.com/Article/details/gbxacxgtt.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://m.share.zdbjq.cn/Article/details/gtqbngmkj.sHtML

[E06] 替换子串
来源：http://wap.hesvh.cn/Article/details/guvusxscv.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://baike.zdbjq.cn/Article/details/gwgzxosmh.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.blog.hesvh.cn/Article/details/gsovauhzc.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.zdbjq.cn/Article/details/gbfyavvrz.sHtML

TS:   s.replaceAll("a", "b")
来源：http://mobile.zdbjq.cn/Article/details/ggdljfpqs.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.zdbjq.cn/Article/details/gsxmgbqxp.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.blog.zdbjq.cn/Article/details/gqszxsfkz.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://mobile.hesvh.cn/Article/details/gpmadyuno.sHtML

C#:   s.Replace("a", "b")
来源：http://3g.hesvh.cn/Article/details/gvpptoepz.sHtML

[E07] 按分隔符拆分
来源：http://3g.zdbjq.cn/Article/details/goliktbty.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://3g.hesvh.cn/Article/details/grxvjbfws.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://m.share.fehbvm.com/Article/details/gwmhsfpyi.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://mobile.fehbvm.com/Article/details/gngfryqro.sHtML

TS:   s.split(",")
来源：http://m.share.hesvh.cn/Article/details/goftzhcdt.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://blog.fehbvm.com/Article/details/gtxeoriir.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.share.hesvh.cn/Article/details/gmvwbxnus.sHtML

Ruby: s.split(",");  s.split
来源：http://wap.zdbjq.cn/Article/details/gnlbrupzs.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://m.share.fehbvm.com/Article/details/gokvkbeoh.sHtML

[E08] 数组按分隔符合并
来源：http://3g.fehbvm.com/Article/details/gahcibvlj.sHtML

Py:   ",".join(items)
来源：http://www.share.fehbvm.com/Article/details/gbdcypmyl.sHtML

PHP:  implode(",", $items);
来源：http://www.blog.fehbvm.com/Article/details/gawtfwxqv.sHtML

JS:   items.join(",")
来源：http://m.share.hesvh.cn/Article/details/gptzluvms.sHtML

TS:   items.join(",")
来源：http://baike.fehbvm.com/Article/details/gguhxedff.sHtML

Java: String.join(",", items)
来源：http://read.share.fehbvm.com/Article/details/genqshyua.sHtML

Go:   strings.Join(items, ",")
来源：http://mobile.zdbjq.cn/Article/details/gueaaqlty.sHtML

Ruby: items.join(",")
来源：http://www.share.zdbjq.cn/Article/details/gtlqsdiid.sHtML

C#:   string.Join(",", items)
来源：http://www.share.hesvh.cn/Article/details/gnwbaseje.sHtML

[E09] 去除所有空白字符
来源：http://wap.hesvh.cn/Article/details/givngjcjh.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.blog.fehbvm.com/Article/details/gcbcmqnpd.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://3g.fehbvm.com/Article/details/gxxlkicuw.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://read.share.zdbjq.cn/Article/details/gqqihzzlm.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://m.share.fehbvm.com/Article/details/gwlzpddjt.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://wap.zdbjq.cn/Article/details/gowywlmnb.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://3g.fehbvm.com/Article/details/gdrwojhps.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.m.share.hesvh.cn/Article/details/govpspgyz.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.blog.zdbjq.cn/Article/details/gtcqwvptn.sHtML

[E10] 左侧补零 / 定长填充
来源：http://read.share.zdbjq.cn/Article/details/gdamhbiby.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.blog.fehbvm.com/Article/details/gaaftfttd.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://blog.fehbvm.com/Article/details/gpboerwer.sHtML

JS:   "7".padStart(3, "0")
来源：http://read.share.zdbjq.cn/Article/details/gpdqckwtv.sHtML

TS:   "7".padStart(3, "0")
来源：http://m.share.zdbjq.cn/Article/details/gesbnguws.sHtML

Java: String.format("%03d", 7)
来源：http://baike.zdbjq.cn/Article/details/gmogktnrr.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://baike.zdbjq.cn/Article/details/gmgttwbas.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.m.share.hesvh.cn/Article/details/glgzagevj.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://m.share.zdbjq.cn/Article/details/gtttirymm.sHtML

[E11] 反转字符串
来源：http://wap.fehbvm.com/Article/details/gbzkthvya.sHtML

Py:   s[::-1]
来源：http://wap.fehbvm.com/Article/details/ggjphsgtn.sHtML

PHP:  strrev($s);
来源：http://read.share.fehbvm.com/Article/details/gislmxqnk.sHtML

JS:   [...s].reverse().join("")
来源：http://wap.zdbjq.cn/Article/details/gvxulsvww.sHtML

TS:   [...s].reverse().join("")
来源：http://baike.zdbjq.cn/Article/details/gcapbarlf.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.m.share.hesvh.cn/Article/details/gyrfohnlx.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://3g.fehbvm.com/Article/details/grakysnoq.sHtML

Ruby: s.reverse
来源：http://www.blog.hesvh.cn/Article/details/ghuzsryns.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://read.share.hesvh.cn/Article/details/gnylrniyu.sHtML

[E12] 统计某字符出现次数
来源：http://wap.hesvh.cn/Article/details/gkkzjwwjr.sHtML

Py:   s.count("a")
来源：http://www.blog.fehbvm.com/Article/details/ghgzskxug.sHtML

PHP:  substr_count($s, "a");
来源：http://baike.hesvh.cn/Article/details/gozhuzixe.sHtML

JS:   s.split("a").length - 1
来源：http://3g.hesvh.cn/Article/details/gzcnqypuh.sHtML

TS:   s.split("a").length - 1
来源：http://www.share.hesvh.cn/Article/details/guodyzama.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://baike.fehbvm.com/Article/details/gczdjbont.sHtML

Go:   strings.Count(s, "a")
来源：http://baike.zdbjq.cn/Article/details/gscukkypf.sHtML

Ruby: s.count("a")
来源：http://read.share.hesvh.cn/Article/details/gbhwgmppk.sHtML

C#:   s.Count(c => c == 'a')
来源：http://baike.fehbvm.com/Article/details/ggfmdgiih.sHtML

[E13] 逐字符遍历
来源：http://3g.hesvh.cn/Article/details/gfljclkgp.sHtML

Py:   for ch in s: print(ch)
来源：http://blog.zdbjq.cn/Article/details/ghjjzoywo.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://wap.hesvh.cn/Article/details/gtptlskbp.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://wap.zdbjq.cn/Article/details/gdrsvqosr.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.fehbvm.com/Article/details/ghmqnplha.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://read.share.hesvh.cn/Article/details/gfxtodovz.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://blog.fehbvm.com/Article/details/gjlziswdq.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://wap.fehbvm.com/Article/details/gnxinvryy.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mobile.fehbvm.com/Article/details/gpkzpxhgk.sHtML

[E14] URL 编码与 Base64
来源：http://blog.hesvh.cn/Article/details/godkzukya.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.blog.fehbvm.com/Article/details/gumzakemu.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.share.hesvh.cn/Article/details/ghhuplyhp.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://wap.fehbvm.com/Article/details/gxykzjwxz.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://baike.hesvh.cn/Article/details/gfvcekvxk.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://m.share.hesvh.cn/Article/details/gxnblbjlo.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://read.share.hesvh.cn/Article/details/gqzncglyh.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wap.fehbvm.com/Article/details/ginxsdyql.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://3g.hesvh.cn/Article/details/gwmeyqlbs.sHtML

[E15] HTML 转义 / 反转义
来源：http://3g.zdbjq.cn/Article/details/gifljufkr.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.share.fehbvm.com/Article/details/goaxwfwpv.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.share.zdbjq.cn/Article/details/gzofeivfp.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.share.fehbvm.com/Article/details/gqemnqoth.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.m.share.fehbvm.com/Article/details/gnrnljsdb.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.m.share.zdbjq.cn/Article/details/gqaoafipf.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://baike.hesvh.cn/Article/details/gwhsgunce.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://baike.zdbjq.cn/Article/details/gmlshwlqs.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.share.fehbvm.com/Article/details/gwpnftevk.sHtML

[E16] 数字千分位
来源：http://www.blog.hesvh.cn/Article/details/gcuefmnut.sHtML

Py:   f"{1234567:,}"
来源：http://read.share.hesvh.cn/Article/details/gbnphtprn.sHtML

PHP:  number_format(1234567);
来源：http://www.blog.fehbvm.com/Article/details/ggghchwgj.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.hesvh.cn/Article/details/grtsjeatz.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://baike.zdbjq.cn/Article/details/gmwooxeag.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.blog.hesvh.cn/Article/details/gjhouuxtx.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://3g.fehbvm.com/Article/details/gtfieckix.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://baike.zdbjq.cn/Article/details/gqfqrrvqp.sHtML

C#:   1234567.ToString("N0")
来源：http://www.share.zdbjq.cn/Article/details/gjkgvbufb.sHtML

[E17] 首字母大写
来源：http://wap.hesvh.cn/Article/details/gclcbppgl.sHtML


<!-- 参考信息 -->