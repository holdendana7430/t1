代发 wailian999

PHP:  sort($arr);
来源：http://mobile.fanxiaobao.xyz/Article/details/gxbxigfer.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://baike.fanxiaobao.xyz/Article/details/gvigmtzyw.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://blog.fanxiaobao.xyz/Article/details/gjrpnlvzo.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://m.share.fanxiaobao.xyz/Article/details/gimelapfk.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://blog.fanxiaobao.xyz/Article/details/gykosdejw.sHtML

Ruby: arr.sort
来源：http://blog.fanxiaobao.xyz/Article/details/gcejqsbry.sHtML

C#:   list.Sort();
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkcwqawjo.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://3g.fanxiaobao.xyz/Article/details/glgkkmusy.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://wap.fanxiaobao.xyz/Article/details/ghsacafnj.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.fanxiaobao.xyz/Article/details/ggapnqzhl.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmbfxppie.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.fanxiaobao.xyz/Article/details/grfjszsuh.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://blog.fanxiaobao.xyz/Article/details/gqrefhlnk.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.share.fanxiaobao.xyz/Article/details/gbvfnomgh.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.blog.fanxiaobao.xyz/Article/details/ginaplvzd.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.share.fanxiaobao.xyz/Article/details/gmfukqyoe.sHtML

[D11] 反转数组
来源：http://3g.fanxiaobao.xyz/Article/details/glyoxqhzx.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnaubtmzj.sHtML

PHP:  array_reverse($arr);
来源：http://m.share.fanxiaobao.xyz/Article/details/ggwgivtwy.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://baike.fanxiaobao.xyz/Article/details/gzviufxqg.sHtML

TS:   [...arr].reverse();
来源：http://read.share.fanxiaobao.xyz/Article/details/gdpefsbqv.sHtML

Java: Collections.reverse(list);
来源：http://3g.fanxiaobao.xyz/Article/details/gpfblbekc.sHtML

Go:   slices.Reverse(arr)
来源：http://blog.fanxiaobao.xyz/Article/details/grjtghimf.sHtML

Ruby: arr.reverse
来源：http://m.share.fanxiaobao.xyz/Article/details/gnvntolwv.sHtML

C#:   list.Reverse();
来源：http://read.share.fanxiaobao.xyz/Article/details/girgyohzw.sHtML

[D12] 查找元素下标
来源：http://wap.fanxiaobao.xyz/Article/details/glvtwwdel.sHtML

Py:   arr.index(x);  x in arr
来源：http://3g.fanxiaobao.xyz/Article/details/gjjyobfkj.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://baike.fanxiaobao.xyz/Article/details/gyyfwhfkt.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.fanxiaobao.xyz/Article/details/gvnbbcozr.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.fanxiaobao.xyz/Article/details/gswbhbbys.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.share.fanxiaobao.xyz/Article/details/gzaukkumi.sHtML

Go:   slices.Index(arr, x)
来源：http://wap.fanxiaobao.xyz/Article/details/gahfgvgom.sHtML

Ruby: arr.index(x)
来源：http://blog.fanxiaobao.xyz/Article/details/gafeiqwyw.sHtML

C#:   list.IndexOf(x);
来源：http://read.share.fanxiaobao.xyz/Article/details/gynjepouu.sHtML

[D13] 过滤（保留满足条件的）
来源：http://blog.fanxiaobao.xyz/Article/details/gzjomkitz.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://baike.fanxiaobao.xyz/Article/details/gidptbzjj.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://mobile.fanxiaobao.xyz/Article/details/goblcsffz.sHtML

JS:   arr.filter(x => x > 3)
来源：http://mobile.fanxiaobao.xyz/Article/details/gxinkliun.sHtML

TS:   arr.filter(x => x > 3)
来源：http://3g.fanxiaobao.xyz/Article/details/gzddfjdqa.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wap.fanxiaobao.xyz/Article/details/gveqhygaz.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://baike.fanxiaobao.xyz/Article/details/gjjrjskex.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjvutsoue.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://baike.fanxiaobao.xyz/Article/details/glouzudii.sHtML

[D14] 映射转换（每个元素变形）
来源：http://wap.fanxiaobao.xyz/Article/details/grpepydxi.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://3g.fanxiaobao.xyz/Article/details/gcthluzkl.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://3g.fanxiaobao.xyz/Article/details/gnuzwmtjr.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvlefzedd.sHtML

TS:   arr.map(x => x * 2)
来源：http://m.share.fanxiaobao.xyz/Article/details/gyanpvhao.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://baike.fanxiaobao.xyz/Article/details/ggqkswawv.sHtML

Go:   // 手写循环
来源：http://wap.fanxiaobao.xyz/Article/details/gimdgopqd.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://3g.fanxiaobao.xyz/Article/details/geikjfizx.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.share.fanxiaobao.xyz/Article/details/guucrupjx.sHtML

[D15] 去重
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghgjtztum.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://m.share.fanxiaobao.xyz/Article/details/gphidwjpi.sHtML

PHP:  array_unique($arr);
来源：http://wap.fanxiaobao.xyz/Article/details/gseetcsyl.sHtML

JS:   [...new Set(arr)]
来源：http://m.share.fanxiaobao.xyz/Article/details/gpasjhfzp.sHtML

TS:   [...new Set(arr)]
来源：http://baike.fanxiaobao.xyz/Article/details/grntajbyz.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://baike.fanxiaobao.xyz/Article/details/gsjlzdljn.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwcemnxac.sHtML

Ruby: arr.uniq
来源：http://m.share.fanxiaobao.xyz/Article/details/glovippxw.sHtML

C#:   list.Distinct().ToList()
来源：http://3g.fanxiaobao.xyz/Article/details/gqgtdyiwv.sHtML

[D16] 求和与平均值
来源：http://m.share.fanxiaobao.xyz/Article/details/gectxhqur.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxwdisrki.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://read.share.fanxiaobao.xyz/Article/details/gblwqnehk.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.fanxiaobao.xyz/Article/details/gdqyfhynu.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.fanxiaobao.xyz/Article/details/gscrovxta.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://wap.fanxiaobao.xyz/Article/details/gacfsliqw.sHtML

Go:   // 手写循环累加
来源：http://www.share.fanxiaobao.xyz/Article/details/gsyfrdrim.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://3g.fanxiaobao.xyz/Article/details/gvhjucaed.sHtML

C#:   list.Sum();  list.Average()
来源：http://wap.fanxiaobao.xyz/Article/details/gqkhnkevg.sHtML

[D17] 最大值与最小值
来源：http://read.share.fanxiaobao.xyz/Article/details/gjcccuvaq.sHtML

Py:   max(arr);  min(arr)
来源：http://m.share.fanxiaobao.xyz/Article/details/gplbsmvtp.sHtML

PHP:  max($arr);  min($arr);
来源：http://m.share.fanxiaobao.xyz/Article/details/gpwlxymiu.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://read.share.fanxiaobao.xyz/Article/details/gsoiiafcq.sHtML

TS:   Math.max(...arr);
来源：http://blog.fanxiaobao.xyz/Article/details/grltkoxbe.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://read.share.fanxiaobao.xyz/Article/details/gdykepksw.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzzsjactr.sHtML

Ruby: arr.max;  arr.min
来源：http://wap.fanxiaobao.xyz/Article/details/gdxlgkhlp.sHtML

C#:   list.Max();  list.Min()
来源：http://3g.fanxiaobao.xyz/Article/details/gmbfuzbau.sHtML

[D18] 扁平化嵌套数组
来源：http://wap.fanxiaobao.xyz/Article/details/gjpdaenfe.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wap.fanxiaobao.xyz/Article/details/gstfbpkol.sHtML

PHP:  array_merge(...$nested);
来源：http://3g.fanxiaobao.xyz/Article/details/gevajlsqj.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mobile.fanxiaobao.xyz/Article/details/gzihesndy.sHtML

TS:   nested.flat();
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnbpesafy.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gejwqvdyz.sHtML

Go:   // 手写双层循环
来源：http://mobile.fanxiaobao.xyz/Article/details/gfoibphwj.sHtML

Ruby: nested.flatten
来源：http://read.share.fanxiaobao.xyz/Article/details/guurzlegt.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvpkjynxz.sHtML

[D19] 按字段分组
来源：http://3g.fanxiaobao.xyz/Article/details/gpyrdrftk.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkvsfdeju.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wap.fanxiaobao.xyz/Article/details/geoagngmo.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://3g.fanxiaobao.xyz/Article/details/gfsetgqle.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.blog.fanxiaobao.xyz/Article/details/giccpendw.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gynlpsisg.sHtML

Go:   // 手写 map[string][]T
来源：http://www.share.fanxiaobao.xyz/Article/details/grhdzjywa.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://read.share.fanxiaobao.xyz/Article/details/gjuyjhsdq.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://m.share.fanxiaobao.xyz/Article/details/gicyuabfa.sHtML

[D20] 统计每个元素出现次数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaeashqcx.sHtML

Py:   Counter(arr)
来源：http://blog.fanxiaobao.xyz/Article/details/gmptcptyj.sHtML

PHP:  array_count_values($arr);
来源：http://read.share.fanxiaobao.xyz/Article/details/ggqkqbpfn.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.fanxiaobao.xyz/Article/details/giuanzvbv.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.fanxiaobao.xyz/Article/details/gqfrdbrys.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wap.fanxiaobao.xyz/Article/details/gxizzokht.sHtML

Go:   // 手写 map[T]int
来源：http://baike.fanxiaobao.xyz/Article/details/gqsldvsep.sHtML

Ruby: arr.tally
来源：http://3g.fanxiaobao.xyz/Article/details/gimtzhdow.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://blog.fanxiaobao.xyz/Article/details/gwvtcpjyy.sHtML

[D21] 判断是否包含某元素
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwmmzzbub.sHtML

Py:   x in arr
来源：http://m.share.fanxiaobao.xyz/Article/details/gkiorlztj.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.share.fanxiaobao.xyz/Article/details/gzlsgvqks.sHtML

JS:   arr.includes(x)
来源：http://read.share.fanxiaobao.xyz/Article/details/gekwzqtra.sHtML

TS:   arr.includes(x)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghsmfdhyi.sHtML

Java: list.contains(x)
来源：http://mobile.fanxiaobao.xyz/Article/details/gpgplorcy.sHtML

Go:   slices.Contains(arr, x)
来源：http://baike.fanxiaobao.xyz/Article/details/gcbzrktpm.sHtML

Ruby: arr.include?(x)
来源：http://www.share.fanxiaobao.xyz/Article/details/grodjqfdc.sHtML

C#:   list.Contains(x)
来源：http://www.blog.fanxiaobao.xyz/Article/details/grbtahlua.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpeqnkqfe.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://baike.fanxiaobao.xyz/Article/details/gsibkpgdk.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.share.fanxiaobao.xyz/Article/details/gvbbkxhuw.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.share.fanxiaobao.xyz/Article/details/gslijhpba.sHtML

TS:   [...arr];
来源：http://read.share.fanxiaobao.xyz/Article/details/ggbhakfwv.sHtML

Java: new ArrayList<>(list);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggtghzdum.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://wap.fanxiaobao.xyz/Article/details/ghwdfubko.sHtML

Ruby: arr.dup;  arr.clone
来源：http://baike.fanxiaobao.xyz/Article/details/gxylzpydo.sHtML

C#:   new List<int>(list);
来源：http://baike.fanxiaobao.xyz/Article/details/grizgkobj.sHtML

[D23] reduce 累积计算
来源：http://mobile.fanxiaobao.xyz/Article/details/gnhyrbnly.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://baike.fanxiaobao.xyz/Article/details/ggrxdkyjt.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://m.share.fanxiaobao.xyz/Article/details/gkpuyxxdq.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.fanxiaobao.xyz/Article/details/gycuoxcjc.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.fanxiaobao.xyz/Article/details/godjxktic.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://3g.fanxiaobao.xyz/Article/details/gxyqhfniu.sHtML

Go:   // 手写循环
来源：http://read.share.fanxiaobao.xyz/Article/details/gwswnwwoi.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://blog.fanxiaobao.xyz/Article/details/gnnozweep.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://baike.fanxiaobao.xyz/Article/details/gnpbjaquw.sHtML

[D24] 字典 / Map 基本操作
来源：http://mobile.fanxiaobao.xyz/Article/details/gpgenffoq.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://baike.fanxiaobao.xyz/Article/details/gpnvtfusa.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mobile.fanxiaobao.xyz/Article/details/glznwjimg.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.share.fanxiaobao.xyz/Article/details/gvfmxqznk.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://baike.fanxiaobao.xyz/Article/details/gbfjbiuni.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://mobile.fanxiaobao.xyz/Article/details/gqhjtlpib.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://wap.fanxiaobao.xyz/Article/details/gulbatrwd.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://3g.fanxiaobao.xyz/Article/details/gxgjmmips.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.share.fanxiaobao.xyz/Article/details/gktestpsi.sHtML

[D25] Set 集合去重与交并差
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtglqkoyf.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://3g.fanxiaobao.xyz/Article/details/gayuitdya.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mobile.fanxiaobao.xyz/Article/details/gdnyskfdk.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://3g.fanxiaobao.xyz/Article/details/gvnxeyryg.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://baike.fanxiaobao.xyz/Article/details/gbkzhkxti.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://3g.fanxiaobao.xyz/Article/details/ghbhswkoo.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://3g.fanxiaobao.xyz/Article/details/gpuewmapp.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://blog.fanxiaobao.xyz/Article/details/gqvsckcmj.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://wap.fanxiaobao.xyz/Article/details/gnqvajjjt.sHtML

[D26] 数组转字符串
来源：http://baike.fanxiaobao.xyz/Article/details/gexoibukf.sHtML

Py:   ", ".join(map(str, arr))
来源：http://mobile.fanxiaobao.xyz/Article/details/gfncqvlkm.sHtML

PHP:  implode(", ", $arr);
来源：http://www.blog.fanxiaobao.xyz/Article/details/glymwsaiw.sHtML

JS:   arr.join(", ")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gevdfrvfh.sHtML

TS:   arr.join(", ")
来源：http://m.share.fanxiaobao.xyz/Article/details/gknloitbl.sHtML

Java: String.join(", ", list)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcgpvqups.sHtML

Go:   strings.Join(strs, ", ")
来源：http://baike.fanxiaobao.xyz/Article/details/gdrzbrguq.sHtML

Ruby: arr.join(", ")
来源：http://wap.fanxiaobao.xyz/Article/details/gdubzline.sHtML

C#:   string.Join(", ", list)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtempnfdf.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gydfjdhaw.sHtML

E. 字符串处理
来源：http://blog.fanxiaobao.xyz/Article/details/gefydcnjr.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gdmuwiyzi.sHtML

[E01] 拼接字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmtybolzn.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://3g.fanxiaobao.xyz/Article/details/gbrksfoxo.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghtflfssw.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.fanxiaobao.xyz/Article/details/ggiddbsyn.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpyzggsid.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/govwjkorh.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wap.fanxiaobao.xyz/Article/details/gzxrlfguf.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnijkgakv.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://blog.fanxiaobao.xyz/Article/details/gnqpsxqhf.sHtML

[E02] 重复字符串
来源：http://mobile.fanxiaobao.xyz/Article/details/gygzoeeor.sHtML

Py:   "ab" * 3
来源：http://www.blog.fanxiaobao.xyz/Article/details/guveajsfo.sHtML

PHP:  str_repeat("ab", 3);
来源：http://3g.fanxiaobao.xyz/Article/details/grxjpyipz.sHtML

JS:   "ab".repeat(3)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqpezebcq.sHtML

TS:   "ab".repeat(3)
来源：http://baike.fanxiaobao.xyz/Article/details/gerlxcplu.sHtML

Java: "ab".repeat(3)
来源：http://wap.fanxiaobao.xyz/Article/details/gtfzjnfbn.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://wap.fanxiaobao.xyz/Article/details/gwprfeqgt.sHtML

Ruby: "ab" * 3
来源：http://read.share.fanxiaobao.xyz/Article/details/grwhskmvm.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wap.fanxiaobao.xyz/Article/details/gepuhmqcq.sHtML

[E03] 截取子串
来源：http://mobile.fanxiaobao.xyz/Article/details/gaksshxiq.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://3g.fanxiaobao.xyz/Article/details/gsraeoxfu.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://wap.fanxiaobao.xyz/Article/details/ghjikmmsi.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://baike.fanxiaobao.xyz/Article/details/gziasqofz.sHtML

TS:   s.slice(1, 4)
来源：http://blog.fanxiaobao.xyz/Article/details/gcvtocoad.sHtML

Java: s.substring(1, 4)
来源：http://read.share.fanxiaobao.xyz/Article/details/gztqhlhjm.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.blog.fanxiaobao.xyz/Article/details/glqkzchkt.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gydembcuu.sHtML

C#:   s.Substring(1, 3)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjyrimfez.sHtML

[E04] 查找子串位置
来源：http://www.share.fanxiaobao.xyz/Article/details/gobioyzhe.sHtML

Py:   s.find("x");  s.index("x")
来源：http://baike.fanxiaobao.xyz/Article/details/glgmofglj.sHtML

PHP:  strpos($s, "x");
来源：http://baike.fanxiaobao.xyz/Article/details/gyrkcwufe.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wap.fanxiaobao.xyz/Article/details/gjlboxfdh.sHtML

TS:   s.indexOf("x")
来源：http://www.share.fanxiaobao.xyz/Article/details/gmjfsucfa.sHtML

Java: s.indexOf("x")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gudvqdaxi.sHtML

Go:   strings.Index(s, "x")
来源：http://wap.fanxiaobao.xyz/Article/details/glimfdmje.sHtML

Ruby: s.index("x")
来源：http://3g.fanxiaobao.xyz/Article/details/gmtcfuhnu.sHtML

C#:   s.IndexOf("x")
来源：http://m.share.fanxiaobao.xyz/Article/details/gbvzrowmc.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://3g.fanxiaobao.xyz/Article/details/ginswvbwo.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gerujawxc.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wap.fanxiaobao.xyz/Article/details/gtazyeywd.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.fanxiaobao.xyz/Article/details/gujmxhoxv.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://3g.fanxiaobao.xyz/Article/details/gayoqomat.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.fanxiaobao.xyz/Article/details/gdcrewvty.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://m.share.fanxiaobao.xyz/Article/details/gwdhzubgx.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://wap.fanxiaobao.xyz/Article/details/gjqomlkni.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://m.share.fanxiaobao.xyz/Article/details/gcqsxsdhg.sHtML

[E06] 替换子串
来源：http://blog.fanxiaobao.xyz/Article/details/gprhirpey.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gthszkbnj.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://m.share.fanxiaobao.xyz/Article/details/gpxohnfsi.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gghdcspyj.sHtML

TS:   s.replaceAll("a", "b")
来源：http://mobile.fanxiaobao.xyz/Article/details/gajdaaupj.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gusejaqwr.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbqsxlztg.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://blog.fanxiaobao.xyz/Article/details/gbamhakwm.sHtML

C#:   s.Replace("a", "b")
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggpmgrjet.sHtML

[E07] 按分隔符拆分
来源：http://wap.fanxiaobao.xyz/Article/details/gisdpwwak.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://m.share.fanxiaobao.xyz/Article/details/ggaxtejwj.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://mobile.fanxiaobao.xyz/Article/details/gepmfmpvh.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.share.fanxiaobao.xyz/Article/details/gdptprlro.sHtML

TS:   s.split(",")
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggyrhzzii.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvynknatc.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://mobile.fanxiaobao.xyz/Article/details/gkjajobse.sHtML

Ruby: s.split(",");  s.split
来源：http://blog.fanxiaobao.xyz/Article/details/glaftqbyl.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wap.fanxiaobao.xyz/Article/details/gidmwyqhw.sHtML

[E08] 数组按分隔符合并
来源：http://mobile.fanxiaobao.xyz/Article/details/gfzmhogmd.sHtML

Py:   ",".join(items)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gindysjqp.sHtML

PHP:  implode(",", $items);
来源：http://www.blog.fanxiaobao.xyz/Article/details/goljnymli.sHtML

JS:   items.join(",")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gblosjfik.sHtML

TS:   items.join(",")
来源：http://mobile.fanxiaobao.xyz/Article/details/gkcltkxvc.sHtML

Java: String.join(",", items)
来源：http://read.share.fanxiaobao.xyz/Article/details/gjaryjqpr.sHtML

Go:   strings.Join(items, ",")
来源：http://read.share.fanxiaobao.xyz/Article/details/gjrsvsyxf.sHtML

Ruby: items.join(",")
来源：http://read.share.fanxiaobao.xyz/Article/details/gpmdoculs.sHtML

C#:   string.Join(",", items)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gowsnkzlr.sHtML

[E09] 去除所有空白字符
来源：http://blog.fanxiaobao.xyz/Article/details/gjmxumyzh.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://read.share.fanxiaobao.xyz/Article/details/gakhtqnvg.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wap.fanxiaobao.xyz/Article/details/gsscabozw.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfkygiatv.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.share.fanxiaobao.xyz/Article/details/gzronjesk.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://3g.fanxiaobao.xyz/Article/details/geqwuaokz.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gotiijgbh.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://baike.fanxiaobao.xyz/Article/details/gdpynjkhj.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grfanqdih.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gksejzfeo.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://blog.fanxiaobao.xyz/Article/details/gjxyprwxh.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmknvpajn.sHtML

JS:   "7".padStart(3, "0")
来源：http://read.share.fanxiaobao.xyz/Article/details/ggypsjoii.sHtML

TS:   "7".padStart(3, "0")
来源：http://3g.fanxiaobao.xyz/Article/details/gfnbvjmze.sHtML

Java: String.format("%03d", 7)
来源：http://mobile.fanxiaobao.xyz/Article/details/gfsonsdyc.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpgfovbgi.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://m.share.fanxiaobao.xyz/Article/details/gbpipdqfs.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://read.share.fanxiaobao.xyz/Article/details/gdlueeybb.sHtML

[E11] 反转字符串
来源：http://read.share.fanxiaobao.xyz/Article/details/guocqvfah.sHtML

Py:   s[::-1]
来源：http://wap.fanxiaobao.xyz/Article/details/gwcbeiwff.sHtML

PHP:  strrev($s);
来源：http://wap.fanxiaobao.xyz/Article/details/gobhjuyiz.sHtML

JS:   [...s].reverse().join("")
来源：http://3g.fanxiaobao.xyz/Article/details/gtorgbrzf.sHtML

TS:   [...s].reverse().join("")
来源：http://3g.fanxiaobao.xyz/Article/details/gqwmtwslr.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://read.share.fanxiaobao.xyz/Article/details/gwscinppi.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.blog.fanxiaobao.xyz/Article/details/glgwtgvxu.sHtML

Ruby: s.reverse
来源：http://read.share.fanxiaobao.xyz/Article/details/gszetkgmd.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://blog.fanxiaobao.xyz/Article/details/giegjsyof.sHtML

[E12] 统计某字符出现次数
来源：http://mobile.fanxiaobao.xyz/Article/details/gummthzif.sHtML

Py:   s.count("a")
来源：http://wap.fanxiaobao.xyz/Article/details/gsmfwfrrd.sHtML

PHP:  substr_count($s, "a");
来源：http://read.share.fanxiaobao.xyz/Article/details/gaevjqibc.sHtML

JS:   s.split("a").length - 1
来源：http://3g.fanxiaobao.xyz/Article/details/gtfditafp.sHtML

TS:   s.split("a").length - 1
来源：http://baike.fanxiaobao.xyz/Article/details/gnxrhmvuc.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggodhvujn.sHtML

Go:   strings.Count(s, "a")
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghmsqatdv.sHtML

Ruby: s.count("a")
来源：http://wap.fanxiaobao.xyz/Article/details/gticerkge.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcltwxuzk.sHtML

[E13] 逐字符遍历
来源：http://3g.fanxiaobao.xyz/Article/details/gvmbqzswh.sHtML

Py:   for ch in s: print(ch)
来源：http://m.share.fanxiaobao.xyz/Article/details/gkcojmoan.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://mobile.fanxiaobao.xyz/Article/details/grzrdxotk.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.fanxiaobao.xyz/Article/details/gcgsrvefv.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqzftqafg.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gknrpaaui.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://3g.fanxiaobao.xyz/Article/details/gcjoopuns.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.blog.fanxiaobao.xyz/Article/details/givtljpug.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://m.share.fanxiaobao.xyz/Article/details/gbeoohbyu.sHtML

[E14] URL 编码与 Base64
来源：http://read.share.fanxiaobao.xyz/Article/details/gmvundzjp.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbzkvppxl.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.share.fanxiaobao.xyz/Article/details/gzpmiiben.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwdmnfuxi.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://3g.fanxiaobao.xyz/Article/details/ghdjdzulx.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://3g.fanxiaobao.xyz/Article/details/gsbznjovb.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggratmdsn.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtocynrel.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://baike.fanxiaobao.xyz/Article/details/goysnxbyh.sHtML

[E15] HTML 转义 / 反转义
来源：http://mobile.fanxiaobao.xyz/Article/details/gaopkxoox.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://wap.fanxiaobao.xyz/Article/details/gmneolmny.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mobile.fanxiaobao.xyz/Article/details/gdukpzwiy.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://blog.fanxiaobao.xyz/Article/details/gypxopxee.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqcylmuii.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnfrawplc.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfeqklebs.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://blog.fanxiaobao.xyz/Article/details/gohmtfdxv.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjslpkdcn.sHtML

[E16] 数字千分位
来源：http://wap.fanxiaobao.xyz/Article/details/gbtwecoar.sHtML

Py:   f"{1234567:,}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqsoqtiij.sHtML


<!-- 参考信息 -->