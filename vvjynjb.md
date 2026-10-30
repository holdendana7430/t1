代发 wailian999

[D07] 切片 / 取子数组
来源：http://mobile.fanxiaobao.xyz/Article/details/gjhzjuamf.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtcefmbvc.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://wap.fanxiaobao.xyz/Article/details/gpjuwaajp.sHtML

JS:   arr.slice(1, 4);
来源：http://wap.fanxiaobao.xyz/Article/details/ganzpcjir.sHtML

TS:   arr.slice(1, 4);
来源：http://3g.fanxiaobao.xyz/Article/details/gsbkblsjg.sHtML

Java: list.subList(1, 4);
来源：http://m.share.fanxiaobao.xyz/Article/details/gvqpoerzf.sHtML

Go:   arr[1:4]
来源：http://baike.fanxiaobao.xyz/Article/details/gusfaknue.sHtML

Ruby: arr[1, 3]
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqtjytbvf.sHtML

C#:   list.GetRange(1, 3);
来源：http://read.share.fanxiaobao.xyz/Article/details/geobvrory.sHtML

[D08] 合并两个数组
来源：http://baike.fanxiaobao.xyz/Article/details/guitirtzg.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqhngwsyr.sHtML

PHP:  array_merge($a, $b);
来源：http://wap.fanxiaobao.xyz/Article/details/gabramdsr.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://read.share.fanxiaobao.xyz/Article/details/gjncofrjx.sHtML

TS:   [...a, ...b];
来源：http://wap.fanxiaobao.xyz/Article/details/ghqgjhtye.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://mobile.fanxiaobao.xyz/Article/details/goxtfwple.sHtML

Go:   append(a, b...)
来源：http://www.share.fanxiaobao.xyz/Article/details/gvmshphfe.sHtML

Ruby: a + b;  a.concat(b)
来源：http://read.share.fanxiaobao.xyz/Article/details/gdxuzcwbs.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcpicqvlk.sHtML

[D09] 排序（升序）
来源：http://www.share.fanxiaobao.xyz/Article/details/gvsixjtvs.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.fanxiaobao.xyz/Article/details/gllziqdpg.sHtML

PHP:  sort($arr);
来源：http://www.blog.fanxiaobao.xyz/Article/details/glyuyhmcd.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://mobile.fanxiaobao.xyz/Article/details/gpubaxhei.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://read.share.fanxiaobao.xyz/Article/details/gnucvzmpl.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdomdtsjh.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://read.share.fanxiaobao.xyz/Article/details/gzvnhkcow.sHtML

Ruby: arr.sort
来源：http://baike.fanxiaobao.xyz/Article/details/gnlfsoxyc.sHtML

C#:   list.Sort();
来源：http://mobile.fanxiaobao.xyz/Article/details/gqhtvysaz.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghcbihqif.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyfllfhih.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.fanxiaobao.xyz/Article/details/gnapmqbva.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.fanxiaobao.xyz/Article/details/glhhooiny.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.fanxiaobao.xyz/Article/details/gaopkjvcn.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxeoapnki.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://m.share.fanxiaobao.xyz/Article/details/gvirfpati.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://baike.fanxiaobao.xyz/Article/details/ggufaftzm.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wap.fanxiaobao.xyz/Article/details/gbdxrafjl.sHtML

[D11] 反转数组
来源：http://mobile.fanxiaobao.xyz/Article/details/gnahuduvu.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://3g.fanxiaobao.xyz/Article/details/gkhenmqzl.sHtML

PHP:  array_reverse($arr);
来源：http://3g.fanxiaobao.xyz/Article/details/gkgdsoied.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://m.share.fanxiaobao.xyz/Article/details/gousxvfaj.sHtML

TS:   [...arr].reverse();
来源：http://mobile.fanxiaobao.xyz/Article/details/gtdnfhmqy.sHtML

Java: Collections.reverse(list);
来源：http://mobile.fanxiaobao.xyz/Article/details/gcddjgmhw.sHtML

Go:   slices.Reverse(arr)
来源：http://wap.fanxiaobao.xyz/Article/details/gitlseqbu.sHtML

Ruby: arr.reverse
来源：http://m.share.fanxiaobao.xyz/Article/details/gghdolvhq.sHtML

C#:   list.Reverse();
来源：http://mobile.fanxiaobao.xyz/Article/details/ggoyxsafu.sHtML

[D12] 查找元素下标
来源：http://mobile.fanxiaobao.xyz/Article/details/gijasaljk.sHtML

Py:   arr.index(x);  x in arr
来源：http://mobile.fanxiaobao.xyz/Article/details/gxceawgzz.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://m.share.fanxiaobao.xyz/Article/details/gwjyjnrxu.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.fanxiaobao.xyz/Article/details/gjvsqoljg.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.fanxiaobao.xyz/Article/details/ggtggjpaa.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://blog.fanxiaobao.xyz/Article/details/gdeayvgsh.sHtML

Go:   slices.Index(arr, x)
来源：http://m.share.fanxiaobao.xyz/Article/details/gkljvvmsw.sHtML

Ruby: arr.index(x)
来源：http://mobile.fanxiaobao.xyz/Article/details/gyecmkbpv.sHtML

C#:   list.IndexOf(x);
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggzddvxbw.sHtML

[D13] 过滤（保留满足条件的）
来源：http://3g.fanxiaobao.xyz/Article/details/glaodtnew.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvvqxoahh.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.blog.fanxiaobao.xyz/Article/details/goiikvgen.sHtML

JS:   arr.filter(x => x > 3)
来源：http://m.share.fanxiaobao.xyz/Article/details/gqqdbbzan.sHtML

TS:   arr.filter(x => x > 3)
来源：http://m.share.fanxiaobao.xyz/Article/details/gjphhnkif.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://read.share.fanxiaobao.xyz/Article/details/goxsnrwjk.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://blog.fanxiaobao.xyz/Article/details/gmfflokvd.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://wap.fanxiaobao.xyz/Article/details/gzncrhdss.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyqtbbuhs.sHtML

[D14] 映射转换（每个元素变形）
来源：http://3g.fanxiaobao.xyz/Article/details/gvsywoycv.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wap.fanxiaobao.xyz/Article/details/gmqxxuait.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mobile.fanxiaobao.xyz/Article/details/gxqdednhi.sHtML

JS:   arr.map(x => x * 2)
来源：http://baike.fanxiaobao.xyz/Article/details/guuudcqef.sHtML

TS:   arr.map(x => x * 2)
来源：http://blog.fanxiaobao.xyz/Article/details/ggypjphxp.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnotdflfv.sHtML

Go:   // 手写循环
来源：http://mobile.fanxiaobao.xyz/Article/details/gfirrbwti.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://baike.fanxiaobao.xyz/Article/details/gbaccuhnp.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.share.fanxiaobao.xyz/Article/details/gxvrhxbvx.sHtML

[D15] 去重
来源：http://blog.fanxiaobao.xyz/Article/details/gxiipdtav.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://m.share.fanxiaobao.xyz/Article/details/gtmhhbmpf.sHtML

PHP:  array_unique($arr);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giudeaneu.sHtML

JS:   [...new Set(arr)]
来源：http://read.share.fanxiaobao.xyz/Article/details/gdzfyorqg.sHtML

TS:   [...new Set(arr)]
来源：http://www.share.fanxiaobao.xyz/Article/details/gbtcvhusw.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://3g.fanxiaobao.xyz/Article/details/gmowuqzqk.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://read.share.fanxiaobao.xyz/Article/details/gsuuafkzq.sHtML

Ruby: arr.uniq
来源：http://read.share.fanxiaobao.xyz/Article/details/gzfovpulw.sHtML

C#:   list.Distinct().ToList()
来源：http://m.share.fanxiaobao.xyz/Article/details/gbalmgqco.sHtML

[D16] 求和与平均值
来源：http://m.share.fanxiaobao.xyz/Article/details/gaxrbxwuj.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://mobile.fanxiaobao.xyz/Article/details/gsvkncndx.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mobile.fanxiaobao.xyz/Article/details/gnonljinn.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.fanxiaobao.xyz/Article/details/gcmhwncwv.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggieiucqq.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://baike.fanxiaobao.xyz/Article/details/griwawayt.sHtML

Go:   // 手写循环累加
来源：http://m.share.fanxiaobao.xyz/Article/details/giejjkxwk.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://blog.fanxiaobao.xyz/Article/details/glpxgyywt.sHtML

C#:   list.Sum();  list.Average()
来源：http://m.share.fanxiaobao.xyz/Article/details/gdplzhpvi.sHtML

[D17] 最大值与最小值
来源：http://wap.fanxiaobao.xyz/Article/details/gfhjghtyp.sHtML

Py:   max(arr);  min(arr)
来源：http://m.share.fanxiaobao.xyz/Article/details/gkqqjjwua.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsibxemik.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://read.share.fanxiaobao.xyz/Article/details/gxmximejz.sHtML

TS:   Math.max(...arr);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyzhlljzp.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://3g.fanxiaobao.xyz/Article/details/grlfeljmw.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://read.share.fanxiaobao.xyz/Article/details/gzodamytg.sHtML

Ruby: arr.max;  arr.min
来源：http://www.blog.fanxiaobao.xyz/Article/details/grrllnnik.sHtML

C#:   list.Max();  list.Min()
来源：http://baike.fanxiaobao.xyz/Article/details/gjbjsvymh.sHtML

[D18] 扁平化嵌套数组
来源：http://mobile.fanxiaobao.xyz/Article/details/gexahzrlr.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://baike.fanxiaobao.xyz/Article/details/gjoyyxmul.sHtML

PHP:  array_merge(...$nested);
来源：http://blog.fanxiaobao.xyz/Article/details/gxlpzblys.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://3g.fanxiaobao.xyz/Article/details/ghckphtnc.sHtML

TS:   nested.flat();
来源：http://www.blog.fanxiaobao.xyz/Article/details/gythztefn.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://m.share.fanxiaobao.xyz/Article/details/ghaltzcef.sHtML

Go:   // 手写双层循环
来源：http://mobile.fanxiaobao.xyz/Article/details/gzxxpkrcd.sHtML

Ruby: nested.flatten
来源：http://blog.fanxiaobao.xyz/Article/details/gmnoadkvz.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://baike.fanxiaobao.xyz/Article/details/ggtxvqgmm.sHtML

[D19] 按字段分组
来源：http://read.share.fanxiaobao.xyz/Article/details/gavcujpfn.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://3g.fanxiaobao.xyz/Article/details/gmzubgmhu.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://3g.fanxiaobao.xyz/Article/details/gxbswkily.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://baike.fanxiaobao.xyz/Article/details/geugdjdfu.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://3g.fanxiaobao.xyz/Article/details/gwdzbradj.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://baike.fanxiaobao.xyz/Article/details/gaebvokfa.sHtML

Go:   // 手写 map[string][]T
来源：http://wap.fanxiaobao.xyz/Article/details/gzivbvuzz.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://blog.fanxiaobao.xyz/Article/details/gtuonvwnx.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://m.share.fanxiaobao.xyz/Article/details/gzdvnelqj.sHtML

[D20] 统计每个元素出现次数
来源：http://mobile.fanxiaobao.xyz/Article/details/gyybmvjnp.sHtML

Py:   Counter(arr)
来源：http://www.share.fanxiaobao.xyz/Article/details/gcixtxwbb.sHtML

PHP:  array_count_values($arr);
来源：http://read.share.fanxiaobao.xyz/Article/details/gghnzblty.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.fanxiaobao.xyz/Article/details/gnbbduabc.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.fanxiaobao.xyz/Article/details/goxyowhjo.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wap.fanxiaobao.xyz/Article/details/gclynrjyc.sHtML

Go:   // 手写 map[T]int
来源：http://www.share.fanxiaobao.xyz/Article/details/gieebbuww.sHtML

Ruby: arr.tally
来源：http://wap.fanxiaobao.xyz/Article/details/gijfbjfbw.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://read.share.fanxiaobao.xyz/Article/details/gffrsgtlk.sHtML

[D21] 判断是否包含某元素
来源：http://wap.fanxiaobao.xyz/Article/details/gzkvmrdmr.sHtML

Py:   x in arr
来源：http://m.share.fanxiaobao.xyz/Article/details/ggxxlbtmb.sHtML

PHP:  in_array($x, $arr, true);
来源：http://wap.fanxiaobao.xyz/Article/details/gokjbkspd.sHtML

JS:   arr.includes(x)
来源：http://wap.fanxiaobao.xyz/Article/details/gwvusxtad.sHtML

TS:   arr.includes(x)
来源：http://3g.fanxiaobao.xyz/Article/details/ggdfdtafn.sHtML

Java: list.contains(x)
来源：http://baike.fanxiaobao.xyz/Article/details/gyfuwmylm.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gejhstvvk.sHtML

Ruby: arr.include?(x)
来源：http://www.share.fanxiaobao.xyz/Article/details/gyjshdcft.sHtML

C#:   list.Contains(x)
来源：http://m.share.fanxiaobao.xyz/Article/details/ganiypdlj.sHtML

[D22] 复制数组（避免共享引用）
来源：http://baike.fanxiaobao.xyz/Article/details/gacgntedd.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://baike.fanxiaobao.xyz/Article/details/gmcuruxbw.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://m.share.fanxiaobao.xyz/Article/details/gwkwsrnso.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://baike.fanxiaobao.xyz/Article/details/gfhhacazs.sHtML

TS:   [...arr];
来源：http://m.share.fanxiaobao.xyz/Article/details/gpctxuspy.sHtML

Java: new ArrayList<>(list);
来源：http://mobile.fanxiaobao.xyz/Article/details/gkmgpbfsf.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://wap.fanxiaobao.xyz/Article/details/giqebzudx.sHtML

Ruby: arr.dup;  arr.clone
来源：http://m.share.fanxiaobao.xyz/Article/details/gjmvialmw.sHtML

C#:   new List<int>(list);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsllnokjv.sHtML

[D23] reduce 累积计算
来源：http://read.share.fanxiaobao.xyz/Article/details/gfoyonvzi.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://baike.fanxiaobao.xyz/Article/details/goraayacd.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://baike.fanxiaobao.xyz/Article/details/gbdfcmxlu.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gualltdoq.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.fanxiaobao.xyz/Article/details/gjjrokuiq.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.share.fanxiaobao.xyz/Article/details/glfbzaaij.sHtML

Go:   // 手写循环
来源：http://m.share.fanxiaobao.xyz/Article/details/gnlertnqn.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mobile.fanxiaobao.xyz/Article/details/gtufcixty.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyucqjrgl.sHtML

[D24] 字典 / Map 基本操作
来源：http://baike.fanxiaobao.xyz/Article/details/gmrvwpwhy.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnrznvdsg.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gidhdfdnj.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gafupsnrk.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://m.share.fanxiaobao.xyz/Article/details/guswzufyy.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gskgkvfal.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://3g.fanxiaobao.xyz/Article/details/ggjaruxpp.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giwaoyrlt.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gszoozvpd.sHtML

[D25] Set 集合去重与交并差
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grckhgoit.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://mobile.fanxiaobao.xyz/Article/details/guuawguny.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://read.share.fanxiaobao.xyz/Article/details/ggjmctdhu.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wap.fanxiaobao.xyz/Article/details/gxugkgsos.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfxjlcvxx.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://wap.fanxiaobao.xyz/Article/details/gxicjuugu.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmvijamcl.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wap.fanxiaobao.xyz/Article/details/guvoorqex.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://baike.fanxiaobao.xyz/Article/details/gfvtbifno.sHtML

[D26] 数组转字符串
来源：http://www.share.fanxiaobao.xyz/Article/details/gmsazlshc.sHtML

Py:   ", ".join(map(str, arr))
来源：http://baike.fanxiaobao.xyz/Article/details/gdnlgjcmt.sHtML

PHP:  implode(", ", $arr);
来源：http://3g.fanxiaobao.xyz/Article/details/gfsgvxnyz.sHtML

JS:   arr.join(", ")
来源：http://3g.fanxiaobao.xyz/Article/details/giqlseiwk.sHtML

TS:   arr.join(", ")
来源：http://blog.fanxiaobao.xyz/Article/details/gwiyhsdtj.sHtML

Java: String.join(", ", list)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnpcluaya.sHtML

Go:   strings.Join(strs, ", ")
来源：http://blog.fanxiaobao.xyz/Article/details/gxaaacber.sHtML

Ruby: arr.join(", ")
来源：http://www.share.fanxiaobao.xyz/Article/details/gduomjbxe.sHtML

C#:   string.Join(", ", list)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcufxluxs.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gggukayte.sHtML

E. 字符串处理
来源：http://mobile.fanxiaobao.xyz/Article/details/gztxmfytk.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gxrgrqzak.sHtML

[E01] 拼接字符串
来源：http://read.share.fanxiaobao.xyz/Article/details/gvrbukgbd.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.blog.fanxiaobao.xyz/Article/details/grauyculo.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://blog.fanxiaobao.xyz/Article/details/gedivqbhy.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwuqxeszy.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.fanxiaobao.xyz/Article/details/gxvviolxr.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://3g.fanxiaobao.xyz/Article/details/grqhmmwcy.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://3g.fanxiaobao.xyz/Article/details/gcogsfxzv.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://3g.fanxiaobao.xyz/Article/details/gapafbkgv.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfnvbzldt.sHtML

[E02] 重复字符串
来源：http://mobile.fanxiaobao.xyz/Article/details/gnrxrurfu.sHtML

Py:   "ab" * 3
来源：http://www.blog.fanxiaobao.xyz/Article/details/geiwqzzom.sHtML

PHP:  str_repeat("ab", 3);
来源：http://read.share.fanxiaobao.xyz/Article/details/gisqmoegq.sHtML

JS:   "ab".repeat(3)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gomsubfgm.sHtML

TS:   "ab".repeat(3)
来源：http://blog.fanxiaobao.xyz/Article/details/ggnsinvle.sHtML

Java: "ab".repeat(3)
来源：http://www.share.fanxiaobao.xyz/Article/details/gmcnhduyi.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.share.fanxiaobao.xyz/Article/details/gtzvfcfrg.sHtML

Ruby: "ab" * 3
来源：http://3g.fanxiaobao.xyz/Article/details/gzybqgmuf.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://mobile.fanxiaobao.xyz/Article/details/gklgvjurl.sHtML

[E03] 截取子串
来源：http://blog.fanxiaobao.xyz/Article/details/gknszatls.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://m.share.fanxiaobao.xyz/Article/details/gnutxjxqx.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://mobile.fanxiaobao.xyz/Article/details/gjabpytua.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://m.share.fanxiaobao.xyz/Article/details/gxxisqaul.sHtML

TS:   s.slice(1, 4)
来源：http://baike.fanxiaobao.xyz/Article/details/gijwzlcmj.sHtML

Java: s.substring(1, 4)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnjssjike.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://baike.fanxiaobao.xyz/Article/details/gdigqeizb.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://m.share.fanxiaobao.xyz/Article/details/ggmugkugl.sHtML

C#:   s.Substring(1, 3)
来源：http://www.share.fanxiaobao.xyz/Article/details/gepaeaeus.sHtML

[E04] 查找子串位置
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzvogfdqn.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjqdfdfbi.sHtML

PHP:  strpos($s, "x");
来源：http://www.share.fanxiaobao.xyz/Article/details/gaclbuqey.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnkpmyvnv.sHtML

TS:   s.indexOf("x")
来源：http://read.share.fanxiaobao.xyz/Article/details/gcvohrmdu.sHtML

Java: s.indexOf("x")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxfxyqkpy.sHtML

Go:   strings.Index(s, "x")
来源：http://3g.fanxiaobao.xyz/Article/details/gtxvmmazm.sHtML

Ruby: s.index("x")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghiykyogv.sHtML

C#:   s.IndexOf("x")
来源：http://baike.fanxiaobao.xyz/Article/details/gwlbfcdpg.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.blog.fanxiaobao.xyz/Article/details/gikcuagbw.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.share.fanxiaobao.xyz/Article/details/gwcqitfyd.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://baike.fanxiaobao.xyz/Article/details/gkmawexwm.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.fanxiaobao.xyz/Article/details/gewavqdnw.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://mobile.fanxiaobao.xyz/Article/details/gvtbcbnfp.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.fanxiaobao.xyz/Article/details/gmmdndgdj.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.share.fanxiaobao.xyz/Article/details/gbntaypsz.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://baike.fanxiaobao.xyz/Article/details/gidyyjbbb.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://mobile.fanxiaobao.xyz/Article/details/gttgfdxqo.sHtML

[E06] 替换子串
来源：http://baike.fanxiaobao.xyz/Article/details/gxukwpwxh.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://baike.fanxiaobao.xyz/Article/details/gyoaqnrkx.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://baike.fanxiaobao.xyz/Article/details/gbfmnjgrg.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.fanxiaobao.xyz/Article/details/ggpwzrsdq.sHtML

TS:   s.replaceAll("a", "b")
来源：http://3g.fanxiaobao.xyz/Article/details/gyaaqegfj.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqajtejhv.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://blog.fanxiaobao.xyz/Article/details/gwyjawent.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://mobile.fanxiaobao.xyz/Article/details/gpfevmulr.sHtML

C#:   s.Replace("a", "b")
来源：http://baike.fanxiaobao.xyz/Article/details/giffokrxl.sHtML

[E07] 按分隔符拆分
来源：http://m.share.fanxiaobao.xyz/Article/details/gbaikybsh.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wap.fanxiaobao.xyz/Article/details/ggqetqokf.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwkqqjues.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpeipkxmg.sHtML

TS:   s.split(",")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwxefcoqd.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://blog.fanxiaobao.xyz/Article/details/gtrrretmg.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://blog.fanxiaobao.xyz/Article/details/ggnvlwecv.sHtML

Ruby: s.split(",");  s.split
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbahhovid.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://blog.fanxiaobao.xyz/Article/details/gpcefmpoq.sHtML

[E08] 数组按分隔符合并
来源：http://wap.fanxiaobao.xyz/Article/details/gkksctccf.sHtML

Py:   ",".join(items)
来源：http://3g.fanxiaobao.xyz/Article/details/gogrxxpru.sHtML

PHP:  implode(",", $items);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goscfzccw.sHtML

JS:   items.join(",")
来源：http://mobile.fanxiaobao.xyz/Article/details/gunopvxye.sHtML

TS:   items.join(",")
来源：http://blog.fanxiaobao.xyz/Article/details/gmlriqfzw.sHtML

Java: String.join(",", items)
来源：http://mobile.fanxiaobao.xyz/Article/details/gezknjofa.sHtML

Go:   strings.Join(items, ",")
来源：http://wap.fanxiaobao.xyz/Article/details/gfvdkeehv.sHtML

Ruby: items.join(",")
来源：http://m.share.fanxiaobao.xyz/Article/details/gxqssveoi.sHtML

C#:   string.Join(",", items)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvnuplnpn.sHtML

[E09] 去除所有空白字符
来源：http://www.share.fanxiaobao.xyz/Article/details/gmicltryd.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://m.share.fanxiaobao.xyz/Article/details/gojxirbpe.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://read.share.fanxiaobao.xyz/Article/details/gpdoxflij.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://read.share.fanxiaobao.xyz/Article/details/gowsgjvtf.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://baike.fanxiaobao.xyz/Article/details/gzuapurml.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glwgznyyi.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://wap.fanxiaobao.xyz/Article/details/gopmjalsy.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnlcmlrun.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://read.share.fanxiaobao.xyz/Article/details/grfzdqjui.sHtML

[E10] 左侧补零 / 定长填充
来源：http://read.share.fanxiaobao.xyz/Article/details/gmnhhtarq.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://3g.fanxiaobao.xyz/Article/details/ggdpaervp.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://read.share.fanxiaobao.xyz/Article/details/gakjqiqqe.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gehjkyvue.sHtML

TS:   "7".padStart(3, "0")
来源：http://read.share.fanxiaobao.xyz/Article/details/gbwqyeodv.sHtML

Java: String.format("%03d", 7)
来源：http://www.share.fanxiaobao.xyz/Article/details/gqeuqzaec.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://wap.fanxiaobao.xyz/Article/details/gsewzgmrr.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://baike.fanxiaobao.xyz/Article/details/gkltpwwzz.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://m.share.fanxiaobao.xyz/Article/details/gxmmzflql.sHtML

[E11] 反转字符串
来源：http://blog.fanxiaobao.xyz/Article/details/gugbveect.sHtML

Py:   s[::-1]
来源：http://3g.fanxiaobao.xyz/Article/details/grdpbmvhk.sHtML

PHP:  strrev($s);
来源：http://www.share.fanxiaobao.xyz/Article/details/gmawmcujd.sHtML

JS:   [...s].reverse().join("")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyiatmohs.sHtML

TS:   [...s].reverse().join("")
来源：http://www.share.fanxiaobao.xyz/Article/details/gaygntbyt.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfyvyfscm.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://blog.fanxiaobao.xyz/Article/details/gbchpoeru.sHtML

Ruby: s.reverse
来源：http://www.blog.fanxiaobao.xyz/Article/details/geujmbspj.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://read.share.fanxiaobao.xyz/Article/details/gunxuzncf.sHtML

[E12] 统计某字符出现次数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmqkfhxxz.sHtML

Py:   s.count("a")
来源：http://mobile.fanxiaobao.xyz/Article/details/ghwnrardu.sHtML

PHP:  substr_count($s, "a");
来源：http://blog.fanxiaobao.xyz/Article/details/gozfoelbr.sHtML

JS:   s.split("a").length - 1
来源：http://www.share.fanxiaobao.xyz/Article/details/gpxeldmvy.sHtML

TS:   s.split("a").length - 1
来源：http://mobile.fanxiaobao.xyz/Article/details/gwbkposch.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://mobile.fanxiaobao.xyz/Article/details/gyeggozum.sHtML

Go:   strings.Count(s, "a")
来源：http://3g.fanxiaobao.xyz/Article/details/gkcgpixti.sHtML

Ruby: s.count("a")
来源：http://blog.fanxiaobao.xyz/Article/details/gdknjsiut.sHtML

C#:   s.Count(c => c == 'a')
来源：http://m.share.fanxiaobao.xyz/Article/details/gabjzmalw.sHtML

[E13] 逐字符遍历
来源：http://read.share.fanxiaobao.xyz/Article/details/gqnvgtedw.sHtML

Py:   for ch in s: print(ch)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggbebfklt.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyjrhzmet.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://blog.fanxiaobao.xyz/Article/details/gyffgdzml.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxygvksgu.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsajojgpu.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://m.share.fanxiaobao.xyz/Article/details/ghbjkyoqs.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://mobile.fanxiaobao.xyz/Article/details/geyvvdnfm.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqvlbbkjl.sHtML


<!-- 参考信息 -->