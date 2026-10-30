代发 wailian999

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.blog.zdbjq.cn/Article/details/gkqxvthxo.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.m.share.fehbvm.com/Article/details/gdpxyikjk.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://blog.zdbjq.cn/Article/details/gypspujpw.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.m.share.zdbjq.cn/Article/details/gshiwbsyc.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://wap.fehbvm.com/Article/details/gctidmhgc.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.fehbvm.com/Article/details/giwsbkmmz.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://read.share.hesvh.cn/Article/details/ginraotjm.sHtML

[D06] 数组长度
来源：http://blog.zdbjq.cn/Article/details/gthepwwon.sHtML

Py:   len(arr)
来源：http://read.share.hesvh.cn/Article/details/gxqfdhhom.sHtML

PHP:  count($arr);
来源：http://www.blog.hesvh.cn/Article/details/gahqslxka.sHtML

JS:   arr.length
来源：http://www.blog.hesvh.cn/Article/details/guslaafsm.sHtML

TS:   arr.length
来源：http://mobile.fehbvm.com/Article/details/gydkbtffq.sHtML

Java: list.size();
来源：http://read.share.zdbjq.cn/Article/details/grmkjcfpp.sHtML

Go:   len(arr)
来源：http://3g.hesvh.cn/Article/details/gvoqhefyf.sHtML

Ruby: arr.length; arr.size
来源：http://www.m.share.zdbjq.cn/Article/details/glyktxasi.sHtML

C#:   list.Count;
来源：http://www.blog.zdbjq.cn/Article/details/giotffvtb.sHtML

[D07] 切片 / 取子数组
来源：http://www.blog.hesvh.cn/Article/details/gjwdhwgrb.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mobile.fehbvm.com/Article/details/ghtbjsckb.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.blog.zdbjq.cn/Article/details/gddtcjfis.sHtML

JS:   arr.slice(1, 4);
来源：http://blog.fehbvm.com/Article/details/gmqtwdyun.sHtML

TS:   arr.slice(1, 4);
来源：http://wap.fehbvm.com/Article/details/gsnyoijql.sHtML

Java: list.subList(1, 4);
来源：http://wap.hesvh.cn/Article/details/gswzuounv.sHtML

Go:   arr[1:4]
来源：http://read.share.zdbjq.cn/Article/details/gkiyxydtx.sHtML

Ruby: arr[1, 3]
来源：http://wap.fehbvm.com/Article/details/glzycvkwl.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.m.share.fehbvm.com/Article/details/gzgecmnke.sHtML

[D08] 合并两个数组
来源：http://www.blog.hesvh.cn/Article/details/gxwhsmqiy.sHtML

Py:   a + b;  a.extend(b)
来源：http://3g.zdbjq.cn/Article/details/gbeebznyw.sHtML

PHP:  array_merge($a, $b);
来源：http://mobile.fehbvm.com/Article/details/gqgtwmdnj.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://read.share.fehbvm.com/Article/details/gmfovrlfp.sHtML

TS:   [...a, ...b];
来源：http://www.share.hesvh.cn/Article/details/gsfvhjwhu.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://read.share.fehbvm.com/Article/details/gvkyiralf.sHtML

Go:   append(a, b...)
来源：http://read.share.hesvh.cn/Article/details/gyzxehzaq.sHtML

Ruby: a + b;  a.concat(b)
来源：http://mobile.zdbjq.cn/Article/details/grukhigjq.sHtML

C#:   a.Concat(b).ToList()
来源：http://blog.fehbvm.com/Article/details/gefshhcon.sHtML

[D09] 排序（升序）
来源：http://www.blog.zdbjq.cn/Article/details/gzjavefmp.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.fehbvm.com/Article/details/gavzjzgnz.sHtML

PHP:  sort($arr);
来源：http://3g.fehbvm.com/Article/details/gnpkzxfed.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://3g.zdbjq.cn/Article/details/grpsodqby.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://mobile.zdbjq.cn/Article/details/gxjtopnpw.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://baike.hesvh.cn/Article/details/gktydzqlc.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.blog.fehbvm.com/Article/details/gehiydkfp.sHtML

Ruby: arr.sort
来源：http://www.m.share.fehbvm.com/Article/details/gbjdpgcnx.sHtML

C#:   list.Sort();
来源：http://read.share.fehbvm.com/Article/details/gqkgyqsgf.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://mobile.zdbjq.cn/Article/details/gncpdqkri.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://baike.zdbjq.cn/Article/details/gjfkbtajm.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.fehbvm.com/Article/details/gvkwwsfwl.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.zdbjq.cn/Article/details/gjecyypiz.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.hesvh.cn/Article/details/gvxgpwsdz.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.blog.fehbvm.com/Article/details/goicvqaqk.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.m.share.hesvh.cn/Article/details/gewqfigij.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://3g.hesvh.cn/Article/details/ghepohygv.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://m.share.fehbvm.com/Article/details/gsxwwjona.sHtML

[D11] 反转数组
来源：http://blog.zdbjq.cn/Article/details/gaawsxqti.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://m.share.fehbvm.com/Article/details/gbbgzaqyc.sHtML

PHP:  array_reverse($arr);
来源：http://www.m.share.hesvh.cn/Article/details/gpdvuljlf.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://blog.fehbvm.com/Article/details/gzazavmqo.sHtML

TS:   [...arr].reverse();
来源：http://read.share.zdbjq.cn/Article/details/gberqqkvo.sHtML

Java: Collections.reverse(list);
来源：http://m.share.fehbvm.com/Article/details/gnbextbbr.sHtML

Go:   slices.Reverse(arr)
来源：http://www.share.fehbvm.com/Article/details/gbcbnmtfu.sHtML

Ruby: arr.reverse
来源：http://mobile.fehbvm.com/Article/details/ggbvjhuwb.sHtML

C#:   list.Reverse();
来源：http://www.m.share.hesvh.cn/Article/details/guvuioxcb.sHtML

[D12] 查找元素下标
来源：http://m.share.fehbvm.com/Article/details/gwqjxfvke.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.share.fehbvm.com/Article/details/gpwtgkkbf.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://mobile.hesvh.cn/Article/details/ghfabiqbg.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.hesvh.cn/Article/details/gklhyyuvn.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.zdbjq.cn/Article/details/gnzrieyft.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.blog.zdbjq.cn/Article/details/gwftpsawr.sHtML

Go:   slices.Index(arr, x)
来源：http://baike.hesvh.cn/Article/details/gnqqrrvgp.sHtML

Ruby: arr.index(x)
来源：http://wap.fehbvm.com/Article/details/gufzidtpb.sHtML

C#:   list.IndexOf(x);
来源：http://www.m.share.fehbvm.com/Article/details/gtezgoiel.sHtML

[D13] 过滤（保留满足条件的）
来源：http://read.share.fehbvm.com/Article/details/guwlkyrrc.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.share.hesvh.cn/Article/details/gnapvsviq.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://blog.fehbvm.com/Article/details/gecikyvam.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.blog.hesvh.cn/Article/details/grcjlrniu.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.blog.hesvh.cn/Article/details/gjjrzrqkp.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mobile.zdbjq.cn/Article/details/gopxtmyem.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://read.share.zdbjq.cn/Article/details/gsabfokok.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.share.zdbjq.cn/Article/details/gfdqtbusr.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://wap.hesvh.cn/Article/details/gxgosxtvn.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.m.share.fehbvm.com/Article/details/gibqmvyie.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mobile.zdbjq.cn/Article/details/gohbozasm.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://read.share.hesvh.cn/Article/details/gsevatvnf.sHtML

JS:   arr.map(x => x * 2)
来源：http://blog.zdbjq.cn/Article/details/grbgivazn.sHtML

TS:   arr.map(x => x * 2)
来源：http://baike.hesvh.cn/Article/details/grqvapijo.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.blog.zdbjq.cn/Article/details/gmduwctxh.sHtML

Go:   // 手写循环
来源：http://read.share.zdbjq.cn/Article/details/gkikbfeed.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://wap.fehbvm.com/Article/details/gxviirecn.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://3g.hesvh.cn/Article/details/gzwndkhel.sHtML

[D15] 去重
来源：http://mobile.fehbvm.com/Article/details/ghosviyvv.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://read.share.zdbjq.cn/Article/details/gecxcpyii.sHtML

PHP:  array_unique($arr);
来源：http://www.share.fehbvm.com/Article/details/gbakqokij.sHtML

JS:   [...new Set(arr)]
来源：http://www.share.hesvh.cn/Article/details/gjzlrayqh.sHtML

TS:   [...new Set(arr)]
来源：http://3g.fehbvm.com/Article/details/ghahdkenf.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.share.hesvh.cn/Article/details/guoprabkj.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://wap.hesvh.cn/Article/details/gsufzgehm.sHtML

Ruby: arr.uniq
来源：http://blog.hesvh.cn/Article/details/gtqmwnkiq.sHtML

C#:   list.Distinct().ToList()
来源：http://mobile.fehbvm.com/Article/details/glsvwircd.sHtML

[D16] 求和与平均值
来源：http://www.blog.fehbvm.com/Article/details/gebjcabue.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gehxqrozu.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://3g.zdbjq.cn/Article/details/gzuouooed.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.hesvh.cn/Article/details/gjdpdenwt.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.hesvh.cn/Article/details/gwyyptkpt.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://baike.hesvh.cn/Article/details/gtevdeija.sHtML

Go:   // 手写循环累加
来源：http://wap.fehbvm.com/Article/details/gsuzhzkbb.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.blog.fehbvm.com/Article/details/gdhgsison.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.blog.hesvh.cn/Article/details/goebjzrat.sHtML

[D17] 最大值与最小值
来源：http://blog.hesvh.cn/Article/details/gdevtvvrw.sHtML

Py:   max(arr);  min(arr)
来源：http://read.share.zdbjq.cn/Article/details/getojxkiu.sHtML

PHP:  max($arr);  min($arr);
来源：http://blog.hesvh.cn/Article/details/glqlitrnb.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://blog.fehbvm.com/Article/details/gxwtspzyt.sHtML

TS:   Math.max(...arr);
来源：http://wap.fehbvm.com/Article/details/gshlscytq.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://3g.zdbjq.cn/Article/details/gbnrjbsdx.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.share.zdbjq.cn/Article/details/gunxebqlg.sHtML

Ruby: arr.max;  arr.min
来源：http://www.blog.fehbvm.com/Article/details/gklbunuhf.sHtML

C#:   list.Max();  list.Min()
来源：http://www.blog.hesvh.cn/Article/details/gtxnkbuwf.sHtML

[D18] 扁平化嵌套数组
来源：http://m.share.zdbjq.cn/Article/details/guwbmriay.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.m.share.fehbvm.com/Article/details/gussgxikf.sHtML

PHP:  array_merge(...$nested);
来源：http://wap.hesvh.cn/Article/details/gbkosuycl.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wap.fehbvm.com/Article/details/gmbxawonc.sHtML

TS:   nested.flat();
来源：http://www.blog.zdbjq.cn/Article/details/gxqzigvzi.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://3g.zdbjq.cn/Article/details/gbvjdipyk.sHtML

Go:   // 手写双层循环
来源：http://www.blog.zdbjq.cn/Article/details/gfveetzfd.sHtML

Ruby: nested.flatten
来源：http://www.share.hesvh.cn/Article/details/gwlumhsql.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://m.share.hesvh.cn/Article/details/ghtmzzkmf.sHtML

[D19] 按字段分组
来源：http://read.share.fehbvm.com/Article/details/guljibxpr.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://blog.fehbvm.com/Article/details/gaonxxomx.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.share.hesvh.cn/Article/details/goxyzztpe.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wap.hesvh.cn/Article/details/gjaqcxqtc.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.m.share.zdbjq.cn/Article/details/gylagxbgn.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.m.share.zdbjq.cn/Article/details/gschebydx.sHtML

Go:   // 手写 map[string][]T
来源：http://mobile.hesvh.cn/Article/details/ghzcfpabv.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://read.share.hesvh.cn/Article/details/gugavvyhy.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://baike.fehbvm.com/Article/details/grdetktuk.sHtML

[D20] 统计每个元素出现次数
来源：http://m.share.zdbjq.cn/Article/details/gvkoweffn.sHtML

Py:   Counter(arr)
来源：http://blog.fehbvm.com/Article/details/ghnyprppo.sHtML

PHP:  array_count_values($arr);
来源：http://blog.zdbjq.cn/Article/details/gfpxvpzgx.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.zdbjq.cn/Article/details/gmpiyxshk.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.hesvh.cn/Article/details/govhttoqj.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.blog.hesvh.cn/Article/details/ggjspanyl.sHtML

Go:   // 手写 map[T]int
来源：http://wap.zdbjq.cn/Article/details/ggqplrgao.sHtML

Ruby: arr.tally
来源：http://m.share.fehbvm.com/Article/details/gjjsejeeo.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.share.zdbjq.cn/Article/details/gifnzrmzv.sHtML

[D21] 判断是否包含某元素
来源：http://www.blog.fehbvm.com/Article/details/gqazryhwv.sHtML

Py:   x in arr
来源：http://www.blog.hesvh.cn/Article/details/gkwqhyphc.sHtML

PHP:  in_array($x, $arr, true);
来源：http://mobile.hesvh.cn/Article/details/gfwipiqum.sHtML

JS:   arr.includes(x)
来源：http://baike.zdbjq.cn/Article/details/gxzdiuktg.sHtML

TS:   arr.includes(x)
来源：http://blog.hesvh.cn/Article/details/gqkgepysl.sHtML

Java: list.contains(x)
来源：http://blog.zdbjq.cn/Article/details/gcgflorjv.sHtML

Go:   slices.Contains(arr, x)
来源：http://blog.fehbvm.com/Article/details/gzlnafidb.sHtML

Ruby: arr.include?(x)
来源：http://3g.zdbjq.cn/Article/details/ggdtjbdve.sHtML

C#:   list.Contains(x)
来源：http://m.share.zdbjq.cn/Article/details/gmwfoxlyx.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.m.share.zdbjq.cn/Article/details/gxgwtjsst.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gepxvcikd.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wap.hesvh.cn/Article/details/gecalbngb.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gpgmscgrk.sHtML

TS:   [...arr];
来源：http://www.m.share.zdbjq.cn/Article/details/gpjpnrnya.sHtML

Java: new ArrayList<>(list);
来源：http://read.share.zdbjq.cn/Article/details/gqwlixadp.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://m.share.hesvh.cn/Article/details/glnjkbsfn.sHtML

Ruby: arr.dup;  arr.clone
来源：http://baike.zdbjq.cn/Article/details/gxfxcqbwv.sHtML

C#:   new List<int>(list);
来源：http://www.blog.hesvh.cn/Article/details/gmjwiqggp.sHtML

[D23] reduce 累积计算
来源：http://mobile.fehbvm.com/Article/details/gsovnniit.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://baike.zdbjq.cn/Article/details/geekqyhgf.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://read.share.hesvh.cn/Article/details/gibmpdpmj.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.hesvh.cn/Article/details/glgtdeuyu.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.hesvh.cn/Article/details/gkujhlrme.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://m.share.fehbvm.com/Article/details/gleivwmer.sHtML

Go:   // 手写循环
来源：http://mobile.hesvh.cn/Article/details/gqpeyyghu.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.blog.fehbvm.com/Article/details/gyfxyttdw.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://blog.zdbjq.cn/Article/details/gspeleecl.sHtML

[D24] 字典 / Map 基本操作
来源：http://read.share.zdbjq.cn/Article/details/gqcshdtmc.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://blog.hesvh.cn/Article/details/gajyhhrsb.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://m.share.fehbvm.com/Article/details/gfvwpvqje.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://m.share.zdbjq.cn/Article/details/gzsvkqoff.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://blog.hesvh.cn/Article/details/gjkwksolb.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.m.share.zdbjq.cn/Article/details/gbpxqwyns.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://read.share.zdbjq.cn/Article/details/glzsecgul.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://baike.zdbjq.cn/Article/details/gxlqwwprk.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://baike.fehbvm.com/Article/details/gpzhnydwv.sHtML

[D25] Set 集合去重与交并差
来源：http://read.share.zdbjq.cn/Article/details/gulhckyzi.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wap.fehbvm.com/Article/details/giaomvogu.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://read.share.zdbjq.cn/Article/details/gzbceleet.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://baike.zdbjq.cn/Article/details/guynzwwpv.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.m.share.fehbvm.com/Article/details/gwbruwaxi.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://mobile.zdbjq.cn/Article/details/gmkwqapwk.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.share.zdbjq.cn/Article/details/guvdmldkz.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://m.share.hesvh.cn/Article/details/gahanrzpp.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://baike.fehbvm.com/Article/details/gtvrgvbxx.sHtML

[D26] 数组转字符串
来源：http://wap.fehbvm.com/Article/details/gyucaxgfl.sHtML

Py:   ", ".join(map(str, arr))
来源：http://3g.zdbjq.cn/Article/details/gjhfjheci.sHtML

PHP:  implode(", ", $arr);
来源：http://www.m.share.hesvh.cn/Article/details/geuraorqv.sHtML

JS:   arr.join(", ")
来源：http://mobile.fehbvm.com/Article/details/gizzvwfkx.sHtML

TS:   arr.join(", ")
来源：http://m.share.hesvh.cn/Article/details/gwsgjcnvx.sHtML

Java: String.join(", ", list)
来源：http://m.share.hesvh.cn/Article/details/gxwcpmejg.sHtML

Go:   strings.Join(strs, ", ")
来源：http://read.share.hesvh.cn/Article/details/gtpmcbrzj.sHtML

Ruby: arr.join(", ")
来源：http://3g.zdbjq.cn/Article/details/gqlczdkhx.sHtML

C#:   string.Join(", ", list)
来源：http://mobile.zdbjq.cn/Article/details/gtbjccjgx.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gxjcxyzwp.sHtML

E. 字符串处理
来源：http://www.m.share.zdbjq.cn/Article/details/gzslbhkko.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gawmawgns.sHtML

[E01] 拼接字符串
来源：http://blog.zdbjq.cn/Article/details/glysyodkm.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.m.share.fehbvm.com/Article/details/gwbeyzaav.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://baike.fehbvm.com/Article/details/gmobbsvik.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.hesvh.cn/Article/details/gysfcwmfc.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.fehbvm.com/Article/details/gtkamwpkf.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://blog.hesvh.cn/Article/details/gckqfgqak.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://3g.hesvh.cn/Article/details/gecaqtzyz.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://baike.zdbjq.cn/Article/details/gvxybsrps.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://mobile.fehbvm.com/Article/details/ghfezxqxo.sHtML

[E02] 重复字符串
来源：http://mobile.zdbjq.cn/Article/details/gxdjfrxxg.sHtML

Py:   "ab" * 3
来源：http://blog.zdbjq.cn/Article/details/grdjanfsh.sHtML

PHP:  str_repeat("ab", 3);
来源：http://blog.fehbvm.com/Article/details/gppzhdgel.sHtML

JS:   "ab".repeat(3)
来源：http://www.m.share.fehbvm.com/Article/details/gofekfzki.sHtML

TS:   "ab".repeat(3)
来源：http://read.share.fehbvm.com/Article/details/glbysjjgd.sHtML

Java: "ab".repeat(3)
来源：http://www.share.zdbjq.cn/Article/details/gwstnkeyr.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.share.hesvh.cn/Article/details/gsuwpbacs.sHtML

Ruby: "ab" * 3
来源：http://wap.hesvh.cn/Article/details/gkgmwbdua.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://mobile.zdbjq.cn/Article/details/gcsjiffsr.sHtML

[E03] 截取子串
来源：http://3g.hesvh.cn/Article/details/gmupqnukl.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://baike.hesvh.cn/Article/details/gxdpceftq.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://baike.zdbjq.cn/Article/details/gnoftgyjk.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.m.share.fehbvm.com/Article/details/gucbrhpsu.sHtML

TS:   s.slice(1, 4)
来源：http://wap.fehbvm.com/Article/details/gplixzkef.sHtML

Java: s.substring(1, 4)
来源：http://wap.hesvh.cn/Article/details/gdemmeuwt.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://read.share.fehbvm.com/Article/details/gshptudhc.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://mobile.zdbjq.cn/Article/details/gklhggten.sHtML

C#:   s.Substring(1, 3)
来源：http://read.share.zdbjq.cn/Article/details/glboeaest.sHtML

[E04] 查找子串位置
来源：http://mobile.fehbvm.com/Article/details/gztvjkosh.sHtML

Py:   s.find("x");  s.index("x")
来源：http://wap.hesvh.cn/Article/details/gbsvjzxxt.sHtML

PHP:  strpos($s, "x");
来源：http://m.share.hesvh.cn/Article/details/gqfthkklt.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://m.share.zdbjq.cn/Article/details/gknzujgdk.sHtML

TS:   s.indexOf("x")
来源：http://www.blog.fehbvm.com/Article/details/gxjtfxulw.sHtML

Java: s.indexOf("x")
来源：http://www.m.share.fehbvm.com/Article/details/grbddastn.sHtML

Go:   strings.Index(s, "x")
来源：http://read.share.zdbjq.cn/Article/details/gzbbdwlne.sHtML

Ruby: s.index("x")
来源：http://wap.hesvh.cn/Article/details/gxfflikel.sHtML

C#:   s.IndexOf("x")
来源：http://m.share.hesvh.cn/Article/details/gggvlgjvj.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://blog.hesvh.cn/Article/details/gmqozuqfa.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.m.share.fehbvm.com/Article/details/gtgbyuptq.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.share.zdbjq.cn/Article/details/giohfrplb.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.zdbjq.cn/Article/details/gzgeexgzb.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://mobile.hesvh.cn/Article/details/gafhytort.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.hesvh.cn/Article/details/gjhwssvlw.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.share.zdbjq.cn/Article/details/ggmkopfyk.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://wap.fehbvm.com/Article/details/gxbcsewda.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://m.share.hesvh.cn/Article/details/gpcqworrg.sHtML

[E06] 替换子串
来源：http://read.share.hesvh.cn/Article/details/gxvglnscv.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.share.hesvh.cn/Article/details/ghitylxod.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://read.share.hesvh.cn/Article/details/ghonmhril.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.hesvh.cn/Article/details/gqskvdsyb.sHtML

TS:   s.replaceAll("a", "b")
来源：http://wap.fehbvm.com/Article/details/gxzwyzyga.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.zdbjq.cn/Article/details/gdhhotrdz.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://3g.fehbvm.com/Article/details/grlgsjftz.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://m.share.hesvh.cn/Article/details/grqkyhnzl.sHtML

C#:   s.Replace("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/glqkaqkck.sHtML

[E07] 按分隔符拆分
来源：http://blog.zdbjq.cn/Article/details/gjxylmtxl.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wap.zdbjq.cn/Article/details/gakbikxuh.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://blog.fehbvm.com/Article/details/gkbjuqmpr.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://blog.zdbjq.cn/Article/details/gobwxbmmk.sHtML

TS:   s.split(",")
来源：http://www.share.hesvh.cn/Article/details/gtqpazqek.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://blog.fehbvm.com/Article/details/gbogcihtm.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://m.share.fehbvm.com/Article/details/gkcfrpwnm.sHtML

Ruby: s.split(",");  s.split
来源：http://wap.zdbjq.cn/Article/details/gtllbhdwo.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.blog.hesvh.cn/Article/details/gbupmhfja.sHtML

[E08] 数组按分隔符合并
来源：http://mobile.zdbjq.cn/Article/details/gewlvmzyu.sHtML

Py:   ",".join(items)
来源：http://www.blog.fehbvm.com/Article/details/goypgapmq.sHtML

PHP:  implode(",", $items);
来源：http://baike.hesvh.cn/Article/details/gfhaqksso.sHtML

JS:   items.join(",")
来源：http://read.share.zdbjq.cn/Article/details/guttshkxt.sHtML

TS:   items.join(",")
来源：http://www.share.fehbvm.com/Article/details/gqpvefexx.sHtML

Java: String.join(",", items)
来源：http://www.share.hesvh.cn/Article/details/grpuodsrf.sHtML

Go:   strings.Join(items, ",")
来源：http://www.m.share.hesvh.cn/Article/details/guqtcwojy.sHtML

Ruby: items.join(",")
来源：http://www.share.zdbjq.cn/Article/details/gvmgwoyxf.sHtML

C#:   string.Join(",", items)
来源：http://m.share.fehbvm.com/Article/details/gmirrpxzs.sHtML

[E09] 去除所有空白字符
来源：http://blog.fehbvm.com/Article/details/gnmlffudp.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://read.share.hesvh.cn/Article/details/gnlqhtull.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.blog.fehbvm.com/Article/details/grqlicnbw.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://3g.hesvh.cn/Article/details/gcxfoskws.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://mobile.zdbjq.cn/Article/details/glsgfttrq.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://baike.hesvh.cn/Article/details/gouhzxnjp.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://m.share.hesvh.cn/Article/details/gvmbxwtjz.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://mobile.zdbjq.cn/Article/details/grqyqwjcg.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://baike.fehbvm.com/Article/details/gjypsignr.sHtML

[E10] 左侧补零 / 定长填充
来源：http://m.share.zdbjq.cn/Article/details/gudwyjkac.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.share.fehbvm.com/Article/details/gzzfvvnsy.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://3g.zdbjq.cn/Article/details/gpjeqwyzw.sHtML

JS:   "7".padStart(3, "0")
来源：http://blog.hesvh.cn/Article/details/getayqggz.sHtML

TS:   "7".padStart(3, "0")
来源：http://mobile.fehbvm.com/Article/details/gxxelaeda.sHtML

Java: String.format("%03d", 7)
来源：http://www.share.fehbvm.com/Article/details/gdambmbxp.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.blog.hesvh.cn/Article/details/gdcwjtkaa.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://3g.fehbvm.com/Article/details/gmbedddgc.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://3g.zdbjq.cn/Article/details/gcyzcvaol.sHtML

[E11] 反转字符串
来源：http://www.share.zdbjq.cn/Article/details/gynoqobzb.sHtML

Py:   s[::-1]
来源：http://wap.hesvh.cn/Article/details/gmcigxqzp.sHtML

PHP:  strrev($s);
来源：http://www.blog.fehbvm.com/Article/details/gcywlxynb.sHtML

JS:   [...s].reverse().join("")
来源：http://www.share.fehbvm.com/Article/details/ghxvwuwyd.sHtML

TS:   [...s].reverse().join("")
来源：http://baike.hesvh.cn/Article/details/gvmmikdyk.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://wap.hesvh.cn/Article/details/glyqjtyjb.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://baike.zdbjq.cn/Article/details/glxynqcqb.sHtML

Ruby: s.reverse
来源：http://mobile.fehbvm.com/Article/details/gcyhctquj.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.m.share.zdbjq.cn/Article/details/gibbwrqxa.sHtML

[E12] 统计某字符出现次数
来源：http://www.blog.zdbjq.cn/Article/details/grtdwovxd.sHtML

Py:   s.count("a")
来源：http://wap.fehbvm.com/Article/details/gozduiufd.sHtML


<!-- 参考信息 -->