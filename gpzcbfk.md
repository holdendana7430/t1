代发 wailian999

TS:   [...arr].reverse();
来源：http://www.m.share.zdbjq.cn/Article/details/giunhkhhz.sHtML

Java: Collections.reverse(list);
来源：http://mobile.hesvh.cn/Article/details/glhbfkzog.sHtML

Go:   slices.Reverse(arr)
来源：http://www.share.hesvh.cn/Article/details/gxktxqlbs.sHtML

Ruby: arr.reverse
来源：http://www.blog.zdbjq.cn/Article/details/gtovwapxu.sHtML

C#:   list.Reverse();
来源：http://www.m.share.hesvh.cn/Article/details/gcculxhdl.sHtML

[D12] 查找元素下标
来源：http://mobile.hesvh.cn/Article/details/gyuqcmnno.sHtML

Py:   arr.index(x);  x in arr
来源：http://blog.hesvh.cn/Article/details/glibukhlc.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.blog.fehbvm.com/Article/details/gdvqvjqkh.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.hesvh.cn/Article/details/gzovckxqc.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.zdbjq.cn/Article/details/gcohjzunq.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.share.fehbvm.com/Article/details/gbygrzhiw.sHtML

Go:   slices.Index(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/ghlqnwlba.sHtML

Ruby: arr.index(x)
来源：http://www.share.fehbvm.com/Article/details/giipbfkmd.sHtML

C#:   list.IndexOf(x);
来源：http://mobile.hesvh.cn/Article/details/gmnfuliau.sHtML

[D13] 过滤（保留满足条件的）
来源：http://read.share.hesvh.cn/Article/details/gsbgudgvq.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://3g.hesvh.cn/Article/details/gultlwsfj.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://read.share.fehbvm.com/Article/details/goydwkosc.sHtML

JS:   arr.filter(x => x > 3)
来源：http://3g.hesvh.cn/Article/details/gpgcgsrqg.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.m.share.hesvh.cn/Article/details/goueiqzqi.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wap.zdbjq.cn/Article/details/gwpmrucng.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.blog.zdbjq.cn/Article/details/giizxhnjw.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://m.share.fehbvm.com/Article/details/goheqhamt.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://m.share.zdbjq.cn/Article/details/gxwnvfszq.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.share.zdbjq.cn/Article/details/gitayetqy.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.m.share.zdbjq.cn/Article/details/gbidgutxo.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://read.share.zdbjq.cn/Article/details/gwajwrwjr.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.m.share.fehbvm.com/Article/details/gxhqhebgk.sHtML

TS:   arr.map(x => x * 2)
来源：http://blog.zdbjq.cn/Article/details/gncqdvpdx.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://mobile.hesvh.cn/Article/details/gjonkakbx.sHtML

Go:   // 手写循环
来源：http://mobile.hesvh.cn/Article/details/gejozmrjn.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://baike.hesvh.cn/Article/details/gjgzjsaxv.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.m.share.hesvh.cn/Article/details/glxoterma.sHtML

[D15] 去重
来源：http://www.blog.fehbvm.com/Article/details/gpeihbgbw.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.blog.zdbjq.cn/Article/details/gxhdknilx.sHtML

PHP:  array_unique($arr);
来源：http://blog.fehbvm.com/Article/details/gkemdtfty.sHtML

JS:   [...new Set(arr)]
来源：http://www.share.fehbvm.com/Article/details/gtcfyfspp.sHtML

TS:   [...new Set(arr)]
来源：http://wap.fehbvm.com/Article/details/gxckkwkux.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://mobile.fehbvm.com/Article/details/gwwkdyeij.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://baike.fehbvm.com/Article/details/geynyfhtb.sHtML

Ruby: arr.uniq
来源：http://www.share.zdbjq.cn/Article/details/grjcspgoq.sHtML

C#:   list.Distinct().ToList()
来源：http://m.share.zdbjq.cn/Article/details/gygvqqmsq.sHtML

[D16] 求和与平均值
来源：http://m.share.hesvh.cn/Article/details/ggumycnch.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.blog.hesvh.cn/Article/details/gzuczupce.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://3g.hesvh.cn/Article/details/gabmedfhv.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.hesvh.cn/Article/details/ghvytglyb.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.zdbjq.cn/Article/details/gfdldjtjx.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.share.hesvh.cn/Article/details/geniitcwt.sHtML

Go:   // 手写循环累加
来源：http://blog.zdbjq.cn/Article/details/gfwfytxcj.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://blog.hesvh.cn/Article/details/gbblcxvty.sHtML

C#:   list.Sum();  list.Average()
来源：http://3g.zdbjq.cn/Article/details/gguydrrjs.sHtML

[D17] 最大值与最小值
来源：http://www.share.fehbvm.com/Article/details/gvqjcnfaa.sHtML

Py:   max(arr);  min(arr)
来源：http://baike.hesvh.cn/Article/details/ghhomshuy.sHtML

PHP:  max($arr);  min($arr);
来源：http://m.share.hesvh.cn/Article/details/grylynewu.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.share.hesvh.cn/Article/details/ginfqzywm.sHtML

TS:   Math.max(...arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gcaxxivqt.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://wap.hesvh.cn/Article/details/gebznlxin.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.share.fehbvm.com/Article/details/gaxffryee.sHtML

Ruby: arr.max;  arr.min
来源：http://www.m.share.fehbvm.com/Article/details/gimotavqq.sHtML

C#:   list.Max();  list.Min()
来源：http://3g.fehbvm.com/Article/details/glqytsqco.sHtML

[D18] 扁平化嵌套数组
来源：http://3g.zdbjq.cn/Article/details/gnyrqhshe.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mobile.zdbjq.cn/Article/details/gyopghmsd.sHtML

PHP:  array_merge(...$nested);
来源：http://baike.hesvh.cn/Article/details/gwlnflgzg.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://m.share.hesvh.cn/Article/details/ggsguzkia.sHtML

TS:   nested.flat();
来源：http://blog.hesvh.cn/Article/details/gmixyhzll.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wap.zdbjq.cn/Article/details/gpuyrkwwx.sHtML

Go:   // 手写双层循环
来源：http://mobile.fehbvm.com/Article/details/goanwjoey.sHtML

Ruby: nested.flatten
来源：http://baike.hesvh.cn/Article/details/gknnofwgv.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://3g.fehbvm.com/Article/details/gsqrzapcj.sHtML

[D19] 按字段分组
来源：http://m.share.zdbjq.cn/Article/details/gyfpviexa.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://baike.fehbvm.com/Article/details/getxyplab.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.blog.fehbvm.com/Article/details/gnvxmwlss.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://blog.zdbjq.cn/Article/details/gvdtkjjxj.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.m.share.zdbjq.cn/Article/details/gnmrnzsal.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://wap.hesvh.cn/Article/details/gsgstigre.sHtML

Go:   // 手写 map[string][]T
来源：http://www.share.zdbjq.cn/Article/details/gsqofsuob.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://baike.fehbvm.com/Article/details/gprlbopih.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.share.hesvh.cn/Article/details/gswmawimi.sHtML

[D20] 统计每个元素出现次数
来源：http://www.share.zdbjq.cn/Article/details/ghyffpvek.sHtML

Py:   Counter(arr)
来源：http://wap.hesvh.cn/Article/details/gitejmccv.sHtML

PHP:  array_count_values($arr);
来源：http://mobile.fehbvm.com/Article/details/gusaiwklm.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.hesvh.cn/Article/details/gpksgjarw.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.zdbjq.cn/Article/details/gbtznkljg.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://baike.zdbjq.cn/Article/details/gwsnylxui.sHtML

Go:   // 手写 map[T]int
来源：http://www.blog.fehbvm.com/Article/details/gojdgvzkx.sHtML

Ruby: arr.tally
来源：http://3g.hesvh.cn/Article/details/ggxkbsruh.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://mobile.fehbvm.com/Article/details/gtoghltrb.sHtML

[D21] 判断是否包含某元素
来源：http://mobile.hesvh.cn/Article/details/ghsbbkghx.sHtML

Py:   x in arr
来源：http://mobile.zdbjq.cn/Article/details/gtwlbyaad.sHtML

PHP:  in_array($x, $arr, true);
来源：http://3g.hesvh.cn/Article/details/gdjnhezpn.sHtML

JS:   arr.includes(x)
来源：http://blog.hesvh.cn/Article/details/gcfvwmike.sHtML

TS:   arr.includes(x)
来源：http://m.share.zdbjq.cn/Article/details/guktfpjfx.sHtML

Java: list.contains(x)
来源：http://mobile.fehbvm.com/Article/details/gcaadxian.sHtML

Go:   slices.Contains(arr, x)
来源：http://mobile.hesvh.cn/Article/details/gvazjllll.sHtML

Ruby: arr.include?(x)
来源：http://blog.fehbvm.com/Article/details/grulldvjh.sHtML

C#:   list.Contains(x)
来源：http://www.m.share.fehbvm.com/Article/details/gkmnsvbma.sHtML

[D22] 复制数组（避免共享引用）
来源：http://wap.fehbvm.com/Article/details/gipltflka.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://blog.fehbvm.com/Article/details/gkkbtiugu.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://m.share.zdbjq.cn/Article/details/gygobkmhl.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://baike.hesvh.cn/Article/details/grikyhkgt.sHtML

TS:   [...arr];
来源：http://www.share.zdbjq.cn/Article/details/gwwcpnehd.sHtML

Java: new ArrayList<>(list);
来源：http://www.m.share.hesvh.cn/Article/details/gubvcoifd.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://mobile.fehbvm.com/Article/details/gvxclilup.sHtML

Ruby: arr.dup;  arr.clone
来源：http://read.share.hesvh.cn/Article/details/gqrpokrqm.sHtML

C#:   new List<int>(list);
来源：http://read.share.hesvh.cn/Article/details/gcopdwhov.sHtML

[D23] reduce 累积计算
来源：http://read.share.hesvh.cn/Article/details/gsvvhyuqd.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.m.share.hesvh.cn/Article/details/ghpeqlgdq.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mobile.fehbvm.com/Article/details/gnxzarfhv.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.fehbvm.com/Article/details/gbdgsorxj.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.fehbvm.com/Article/details/gwjecohmz.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://baike.hesvh.cn/Article/details/gzwxzmqpz.sHtML

Go:   // 手写循环
来源：http://read.share.zdbjq.cn/Article/details/goeaqurff.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://3g.zdbjq.cn/Article/details/glxrmclmd.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.share.zdbjq.cn/Article/details/gxwjqjhsh.sHtML

[D24] 字典 / Map 基本操作
来源：http://3g.fehbvm.com/Article/details/glzzvrvty.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://3g.hesvh.cn/Article/details/gpevcybgo.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://3g.fehbvm.com/Article/details/gvxwyxziq.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.m.share.fehbvm.com/Article/details/gijjndudt.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.share.zdbjq.cn/Article/details/gztsxzzvh.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wap.zdbjq.cn/Article/details/guuojbvnj.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://wap.hesvh.cn/Article/details/gjovgtlkc.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://read.share.fehbvm.com/Article/details/gjdjlpxwz.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://blog.zdbjq.cn/Article/details/gftdbaave.sHtML

[D25] Set 集合去重与交并差
来源：http://baike.hesvh.cn/Article/details/gzeszjlli.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.blog.zdbjq.cn/Article/details/gxdeehumb.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.share.zdbjq.cn/Article/details/grbolzoie.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wap.fehbvm.com/Article/details/gmixpkjbt.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://m.share.hesvh.cn/Article/details/gszbhuukg.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gzwcfeshn.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://blog.fehbvm.com/Article/details/gcsplfxag.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mobile.hesvh.cn/Article/details/gvyqecblu.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://wap.fehbvm.com/Article/details/gqsbxzcsr.sHtML

[D26] 数组转字符串
来源：http://mobile.fehbvm.com/Article/details/gfntpicpy.sHtML

Py:   ", ".join(map(str, arr))
来源：http://mobile.zdbjq.cn/Article/details/gligtfuik.sHtML

PHP:  implode(", ", $arr);
来源：http://m.share.zdbjq.cn/Article/details/gvmnyliln.sHtML

JS:   arr.join(", ")
来源：http://wap.fehbvm.com/Article/details/griyvbxox.sHtML

TS:   arr.join(", ")
来源：http://read.share.fehbvm.com/Article/details/gsthehwak.sHtML

Java: String.join(", ", list)
来源：http://www.m.share.zdbjq.cn/Article/details/gsaorzhxl.sHtML

Go:   strings.Join(strs, ", ")
来源：http://3g.zdbjq.cn/Article/details/gtslcxpci.sHtML

Ruby: arr.join(", ")
来源：http://m.share.zdbjq.cn/Article/details/gbeizjsjc.sHtML

C#:   string.Join(", ", list)
来源：http://wap.hesvh.cn/Article/details/gpzkqzrdw.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gwecjljcq.sHtML

E. 字符串处理
来源：http://mobile.fehbvm.com/Article/details/gboakuuun.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gmdinkwtt.sHtML

[E01] 拼接字符串
来源：http://m.share.fehbvm.com/Article/details/gfzmqydyf.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://mobile.zdbjq.cn/Article/details/gzvahwxfm.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.blog.zdbjq.cn/Article/details/guihicjws.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.hesvh.cn/Article/details/gcpvcmctl.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.hesvh.cn/Article/details/gbnpnqoxq.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.m.share.zdbjq.cn/Article/details/gvpkinckc.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://3g.zdbjq.cn/Article/details/godfxuesv.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wap.zdbjq.cn/Article/details/gfolrifzi.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/gcrtjqtvx.sHtML

[E02] 重复字符串
来源：http://wap.fehbvm.com/Article/details/giebwtabu.sHtML

Py:   "ab" * 3
来源：http://read.share.fehbvm.com/Article/details/gixfngqza.sHtML

PHP:  str_repeat("ab", 3);
来源：http://read.share.zdbjq.cn/Article/details/gavnjzjmd.sHtML

JS:   "ab".repeat(3)
来源：http://wap.zdbjq.cn/Article/details/grpgivgxe.sHtML

TS:   "ab".repeat(3)
来源：http://www.blog.zdbjq.cn/Article/details/gxlszgimq.sHtML

Java: "ab".repeat(3)
来源：http://wap.fehbvm.com/Article/details/ggbjwjulb.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://wap.zdbjq.cn/Article/details/gucomtiuo.sHtML

Ruby: "ab" * 3
来源：http://www.blog.fehbvm.com/Article/details/gpwaxehpj.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wap.zdbjq.cn/Article/details/ghzxyrosn.sHtML

[E03] 截取子串
来源：http://3g.hesvh.cn/Article/details/gtajpzetc.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.blog.hesvh.cn/Article/details/gopfljpvh.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://mobile.fehbvm.com/Article/details/glscyprjm.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://3g.hesvh.cn/Article/details/gdrbqvolj.sHtML

TS:   s.slice(1, 4)
来源：http://3g.hesvh.cn/Article/details/gmairbxkf.sHtML

Java: s.substring(1, 4)
来源：http://www.m.share.fehbvm.com/Article/details/gtritcfgl.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://blog.zdbjq.cn/Article/details/gosvuesmx.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.share.zdbjq.cn/Article/details/gavtizquu.sHtML

C#:   s.Substring(1, 3)
来源：http://3g.fehbvm.com/Article/details/gkfyksubs.sHtML

[E04] 查找子串位置
来源：http://m.share.zdbjq.cn/Article/details/gizmokfim.sHtML

Py:   s.find("x");  s.index("x")
来源：http://read.share.hesvh.cn/Article/details/gewkqineb.sHtML

PHP:  strpos($s, "x");
来源：http://wap.hesvh.cn/Article/details/ggvnkqdxf.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wap.zdbjq.cn/Article/details/gbjsmroin.sHtML

TS:   s.indexOf("x")
来源：http://www.m.share.zdbjq.cn/Article/details/gzqiwhcnv.sHtML

Java: s.indexOf("x")
来源：http://www.blog.fehbvm.com/Article/details/glayuurjv.sHtML

Go:   strings.Index(s, "x")
来源：http://blog.hesvh.cn/Article/details/geezrxqbr.sHtML

Ruby: s.index("x")
来源：http://www.share.fehbvm.com/Article/details/gszfpypqo.sHtML

C#:   s.IndexOf("x")
来源：http://www.m.share.zdbjq.cn/Article/details/gksqbvewi.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://baike.zdbjq.cn/Article/details/gvbpdursw.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://mobile.fehbvm.com/Article/details/gsqybdeps.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.m.share.zdbjq.cn/Article/details/gpzazjthj.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.hesvh.cn/Article/details/gnblyzpbb.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://mobile.zdbjq.cn/Article/details/gxutpkkuk.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.fehbvm.com/Article/details/gocgknehv.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wap.hesvh.cn/Article/details/gojwmbttt.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://wap.fehbvm.com/Article/details/gafqhsulu.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.share.fehbvm.com/Article/details/gllbpvssj.sHtML

[E06] 替换子串
来源：http://mobile.fehbvm.com/Article/details/gxncgmtat.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://mobile.fehbvm.com/Article/details/giacxpwfv.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://mobile.zdbjq.cn/Article/details/gdvcqbcfw.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.hesvh.cn/Article/details/ggpsxblge.sHtML

TS:   s.replaceAll("a", "b")
来源：http://wap.fehbvm.com/Article/details/gdhmdpyyy.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.zdbjq.cn/Article/details/gwwdhunwl.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://m.share.hesvh.cn/Article/details/gjacbbbit.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.share.hesvh.cn/Article/details/gwzznvkst.sHtML

C#:   s.Replace("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/gwqtsmrhx.sHtML

[E07] 按分隔符拆分
来源：http://www.blog.hesvh.cn/Article/details/gzcpcrycd.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wap.fehbvm.com/Article/details/gjetupbzq.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://baike.zdbjq.cn/Article/details/gmutlxbjs.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.share.hesvh.cn/Article/details/ggtmcvzqg.sHtML

TS:   s.split(",")
来源：http://www.share.fehbvm.com/Article/details/gqsgzciwx.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://3g.hesvh.cn/Article/details/gmmmhrqjd.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.blog.zdbjq.cn/Article/details/gtbwxhscz.sHtML

Ruby: s.split(",");  s.split
来源：http://m.share.fehbvm.com/Article/details/gtgraakdo.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.m.share.zdbjq.cn/Article/details/gurdnbgdt.sHtML

[E08] 数组按分隔符合并
来源：http://www.blog.fehbvm.com/Article/details/gltvyfaux.sHtML

Py:   ",".join(items)
来源：http://m.share.hesvh.cn/Article/details/ghmezzoky.sHtML

PHP:  implode(",", $items);
来源：http://read.share.fehbvm.com/Article/details/gjywxswii.sHtML

JS:   items.join(",")
来源：http://www.blog.hesvh.cn/Article/details/gexyuviea.sHtML

TS:   items.join(",")
来源：http://read.share.fehbvm.com/Article/details/gptnhrygh.sHtML

Java: String.join(",", items)
来源：http://read.share.fehbvm.com/Article/details/gkcmfehug.sHtML

Go:   strings.Join(items, ",")
来源：http://www.share.zdbjq.cn/Article/details/gvasvmvqn.sHtML

Ruby: items.join(",")
来源：http://www.share.zdbjq.cn/Article/details/gtledzuob.sHtML

C#:   string.Join(",", items)
来源：http://m.share.zdbjq.cn/Article/details/gqogxwlrm.sHtML

[E09] 去除所有空白字符
来源：http://www.m.share.hesvh.cn/Article/details/gyxiufjvx.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.m.share.zdbjq.cn/Article/details/gtcossrwl.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://baike.fehbvm.com/Article/details/gwrxicash.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://baike.zdbjq.cn/Article/details/gsjrnzbrj.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://wap.hesvh.cn/Article/details/gqojvqgwy.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.blog.zdbjq.cn/Article/details/gewpyuobw.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://mobile.hesvh.cn/Article/details/gpmbmgeus.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://blog.zdbjq.cn/Article/details/ghbtlhuwt.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://baike.hesvh.cn/Article/details/glkuqrdnp.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.blog.zdbjq.cn/Article/details/glmswimvy.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://read.share.zdbjq.cn/Article/details/ggaonwshu.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wap.hesvh.cn/Article/details/gkzyctmyz.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.blog.zdbjq.cn/Article/details/gqsurrxdq.sHtML

TS:   "7".padStart(3, "0")
来源：http://read.share.zdbjq.cn/Article/details/gnrlcqhek.sHtML

Java: String.format("%03d", 7)
来源：http://blog.zdbjq.cn/Article/details/gxmeevgth.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://mobile.hesvh.cn/Article/details/gpqwsgjxu.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://wap.hesvh.cn/Article/details/gzecoumky.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://m.share.hesvh.cn/Article/details/gwshwlqum.sHtML

[E11] 反转字符串
来源：http://mobile.fehbvm.com/Article/details/gmdlfxtti.sHtML

Py:   s[::-1]
来源：http://3g.fehbvm.com/Article/details/gadubxlng.sHtML

PHP:  strrev($s);
来源：http://baike.fehbvm.com/Article/details/ggltltosh.sHtML

JS:   [...s].reverse().join("")
来源：http://3g.fehbvm.com/Article/details/gztrbyagx.sHtML

TS:   [...s].reverse().join("")
来源：http://www.blog.fehbvm.com/Article/details/gmmlnleel.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.m.share.zdbjq.cn/Article/details/gxdmsmkpn.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://wap.fehbvm.com/Article/details/gvljkjfio.sHtML

Ruby: s.reverse
来源：http://www.m.share.zdbjq.cn/Article/details/gybwljreb.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://3g.hesvh.cn/Article/details/gzfsfzjpr.sHtML

[E12] 统计某字符出现次数
来源：http://www.share.fehbvm.com/Article/details/gjrelfhsu.sHtML

Py:   s.count("a")
来源：http://blog.fehbvm.com/Article/details/glgmyoebu.sHtML

PHP:  substr_count($s, "a");
来源：http://m.share.zdbjq.cn/Article/details/gapdyxapm.sHtML

JS:   s.split("a").length - 1
来源：http://www.blog.zdbjq.cn/Article/details/gcfnfdnvd.sHtML

TS:   s.split("a").length - 1
来源：http://www.blog.zdbjq.cn/Article/details/gsembkqnf.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.m.share.hesvh.cn/Article/details/gxmolfjus.sHtML

Go:   strings.Count(s, "a")
来源：http://mobile.zdbjq.cn/Article/details/gyuytxtvp.sHtML

Ruby: s.count("a")
来源：http://www.share.hesvh.cn/Article/details/gqxfgnblv.sHtML

C#:   s.Count(c => c == 'a')
来源：http://read.share.zdbjq.cn/Article/details/gujcsbnsp.sHtML

[E13] 逐字符遍历
来源：http://www.blog.hesvh.cn/Article/details/gjqkvjsew.sHtML

Py:   for ch in s: print(ch)
来源：http://blog.hesvh.cn/Article/details/gfppevmyj.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://blog.hesvh.cn/Article/details/gvcmytdhz.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://blog.fehbvm.com/Article/details/gucgnvrgl.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.hesvh.cn/Article/details/gisrqujuw.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://m.share.zdbjq.cn/Article/details/gviyteaat.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://m.share.fehbvm.com/Article/details/grqrvtugt.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://m.share.zdbjq.cn/Article/details/gomlmnkey.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://read.share.zdbjq.cn/Article/details/guxfbspli.sHtML

[E14] URL 编码与 Base64
来源：http://www.share.hesvh.cn/Article/details/ggqhyqrsq.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.share.hesvh.cn/Article/details/glvfnzqgl.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://mobile.hesvh.cn/Article/details/gqssnrjmt.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://baike.fehbvm.com/Article/details/gloazzzvh.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://m.share.zdbjq.cn/Article/details/gxacpcajm.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.m.share.fehbvm.com/Article/details/gbjksxlys.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://wap.zdbjq.cn/Article/details/geaopbqdc.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.share.fehbvm.com/Article/details/gmfcdmrbh.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.m.share.zdbjq.cn/Article/details/ghuraozfo.sHtML

[E15] HTML 转义 / 反转义
来源：http://mobile.zdbjq.cn/Article/details/gfcfqyryo.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://m.share.zdbjq.cn/Article/details/gmmjuttaw.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://m.share.fehbvm.com/Article/details/gxlsminhd.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://blog.zdbjq.cn/Article/details/gdxynrdku.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://baike.zdbjq.cn/Article/details/gdnehxvnz.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mobile.hesvh.cn/Article/details/ggvkokehe.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://3g.zdbjq.cn/Article/details/gukyrvxhx.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://3g.zdbjq.cn/Article/details/gpxmnnvku.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://baike.hesvh.cn/Article/details/gwvlikmrw.sHtML

[E16] 数字千分位
来源：http://baike.zdbjq.cn/Article/details/gugnvhhns.sHtML

Py:   f"{1234567:,}"
来源：http://read.share.zdbjq.cn/Article/details/gobxzlffk.sHtML

PHP:  number_format(1234567);
来源：http://blog.hesvh.cn/Article/details/goyusanlp.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://3g.fehbvm.com/Article/details/gfhwuvvhi.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://mobile.zdbjq.cn/Article/details/gmvrbenvu.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://m.share.zdbjq.cn/Article/details/ggveonldo.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://baike.hesvh.cn/Article/details/ggqvgrylj.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.blog.fehbvm.com/Article/details/gnukejwij.sHtML

C#:   1234567.ToString("N0")
来源：http://www.blog.zdbjq.cn/Article/details/gyvdbtapl.sHtML

[E17] 首字母大写
来源：http://mobile.zdbjq.cn/Article/details/ggykbhyhn.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.blog.fehbvm.com/Article/details/gexywihxl.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://wap.zdbjq.cn/Article/details/gxkobsstf.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.zdbjq.cn/Article/details/glgewzfrj.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.hesvh.cn/Article/details/glaxvqtde.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://3g.hesvh.cn/Article/details/gfconbfbn.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://m.share.fehbvm.com/Article/details/gvwiubewt.sHtML

Ruby: s.capitalize
来源：http://read.share.zdbjq.cn/Article/details/gxpywdlym.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://mobile.zdbjq.cn/Article/details/gbxhhkldf.sHtML

[E18] 模板占位符替换
来源：http://wap.hesvh.cn/Article/details/gpdcgvmwn.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.m.share.zdbjq.cn/Article/details/gdfawmosp.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://wap.zdbjq.cn/Article/details/gtldwriih.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://m.share.zdbjq.cn/Article/details/gocpukcjj.sHtML


<!-- 参考信息 -->