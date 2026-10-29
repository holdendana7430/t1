代发 wailian999

C#:   list.GetRange(1, 3);
来源：http://wap.zdbjq.cn/Article/details/grzxfbdbj.sHtML

[D08] 合并两个数组
来源：http://read.share.hesvh.cn/Article/details/gerqquctv.sHtML

Py:   a + b;  a.extend(b)
来源：http://mobile.fehbvm.com/Article/details/gueqgjprr.sHtML

PHP:  array_merge($a, $b);
来源：http://www.m.share.fehbvm.com/Article/details/gfksgqlrb.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.share.hesvh.cn/Article/details/gshxiscpq.sHtML

TS:   [...a, ...b];
来源：http://read.share.zdbjq.cn/Article/details/gbouosjur.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://baike.hesvh.cn/Article/details/gbtcybyjv.sHtML

Go:   append(a, b...)
来源：http://read.share.zdbjq.cn/Article/details/gapmvbgfo.sHtML

Ruby: a + b;  a.concat(b)
来源：http://read.share.fehbvm.com/Article/details/gkadbrrer.sHtML

C#:   a.Concat(b).ToList()
来源：http://m.share.hesvh.cn/Article/details/gjhmbxrcr.sHtML

[D09] 排序（升序）
来源：http://m.share.fehbvm.com/Article/details/giohycalr.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.fehbvm.com/Article/details/gwnohyjkg.sHtML

PHP:  sort($arr);
来源：http://m.share.fehbvm.com/Article/details/gwzrxefly.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.blog.fehbvm.com/Article/details/gnjeeblnp.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://baike.hesvh.cn/Article/details/gvupxnuct.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://read.share.zdbjq.cn/Article/details/gvbjibosp.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gaihhspbr.sHtML

Ruby: arr.sort
来源：http://blog.hesvh.cn/Article/details/gjcjtoqgu.sHtML

C#:   list.Sort();
来源：http://blog.fehbvm.com/Article/details/gqxriqqub.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://baike.fehbvm.com/Article/details/grgjaflpa.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.blog.hesvh.cn/Article/details/gycjdlfzg.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.zdbjq.cn/Article/details/gmizgjqzh.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.zdbjq.cn/Article/details/guxzrnaee.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.hesvh.cn/Article/details/goyhxtbjr.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://3g.zdbjq.cn/Article/details/gokcgiolk.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://read.share.fehbvm.com/Article/details/gyajvfegx.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://read.share.zdbjq.cn/Article/details/gwmxndvjc.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://read.share.fehbvm.com/Article/details/gsodksrhk.sHtML

[D11] 反转数组
来源：http://blog.hesvh.cn/Article/details/gaotamtcd.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.blog.fehbvm.com/Article/details/gscrfdtig.sHtML

PHP:  array_reverse($arr);
来源：http://blog.zdbjq.cn/Article/details/gqxwkchai.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://baike.zdbjq.cn/Article/details/gpexbmicb.sHtML

TS:   [...arr].reverse();
来源：http://wap.hesvh.cn/Article/details/gwhmxqpmz.sHtML

Java: Collections.reverse(list);
来源：http://wap.fehbvm.com/Article/details/gtnhlhkzc.sHtML

Go:   slices.Reverse(arr)
来源：http://m.share.fehbvm.com/Article/details/gurvxzfne.sHtML

Ruby: arr.reverse
来源：http://m.share.hesvh.cn/Article/details/gqyowpnyc.sHtML

C#:   list.Reverse();
来源：http://wap.fehbvm.com/Article/details/gbpvciyky.sHtML

[D12] 查找元素下标
来源：http://www.m.share.fehbvm.com/Article/details/gxxkvmwfs.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.blog.hesvh.cn/Article/details/glxiklais.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://blog.hesvh.cn/Article/details/gtgtbctev.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.fehbvm.com/Article/details/guerwgczz.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.hesvh.cn/Article/details/gbnrfstwg.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://m.share.zdbjq.cn/Article/details/guybxxskz.sHtML

Go:   slices.Index(arr, x)
来源：http://read.share.hesvh.cn/Article/details/ggayfwudq.sHtML

Ruby: arr.index(x)
来源：http://m.share.hesvh.cn/Article/details/gyiloubty.sHtML

C#:   list.IndexOf(x);
来源：http://mobile.hesvh.cn/Article/details/gdaaqcufk.sHtML

[D13] 过滤（保留满足条件的）
来源：http://3g.zdbjq.cn/Article/details/gmwkazrru.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.m.share.zdbjq.cn/Article/details/gneuxczce.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://blog.fehbvm.com/Article/details/ggjrjqvbd.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.m.share.hesvh.cn/Article/details/gxrursldv.sHtML

TS:   arr.filter(x => x > 3)
来源：http://read.share.hesvh.cn/Article/details/gskjhbvrz.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.m.share.zdbjq.cn/Article/details/gkzdapdgb.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://blog.zdbjq.cn/Article/details/gwhfsuopk.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://blog.hesvh.cn/Article/details/gzpochrmc.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.m.share.hesvh.cn/Article/details/ggmmmzvjj.sHtML

[D14] 映射转换（每个元素变形）
来源：http://wap.fehbvm.com/Article/details/gmlaevcda.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.share.hesvh.cn/Article/details/gwjpntzyq.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mobile.zdbjq.cn/Article/details/gubmkzvns.sHtML

JS:   arr.map(x => x * 2)
来源：http://mobile.zdbjq.cn/Article/details/gcyfuuhwf.sHtML

TS:   arr.map(x => x * 2)
来源：http://3g.zdbjq.cn/Article/details/gvgluvotd.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://blog.zdbjq.cn/Article/details/ggnrxeuit.sHtML

Go:   // 手写循环
来源：http://www.blog.zdbjq.cn/Article/details/gouzjkhge.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.blog.fehbvm.com/Article/details/grjvvsxfz.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.share.hesvh.cn/Article/details/gfnzpxoto.sHtML

[D15] 去重
来源：http://www.blog.fehbvm.com/Article/details/gpganlznx.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://wap.fehbvm.com/Article/details/gopllzojs.sHtML

PHP:  array_unique($arr);
来源：http://m.share.fehbvm.com/Article/details/gnrchlaqs.sHtML

JS:   [...new Set(arr)]
来源：http://read.share.zdbjq.cn/Article/details/gplcjwtjz.sHtML

TS:   [...new Set(arr)]
来源：http://wap.fehbvm.com/Article/details/ghhasrtng.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.blog.zdbjq.cn/Article/details/giwppmhpv.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.share.hesvh.cn/Article/details/guujqoqvz.sHtML

Ruby: arr.uniq
来源：http://mobile.zdbjq.cn/Article/details/gxhfmhycu.sHtML

C#:   list.Distinct().ToList()
来源：http://www.m.share.fehbvm.com/Article/details/gzotnfdis.sHtML

[D16] 求和与平均值
来源：http://blog.hesvh.cn/Article/details/gktfypssl.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.blog.hesvh.cn/Article/details/gcfozaukf.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://m.share.zdbjq.cn/Article/details/gymlzmwsu.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.zdbjq.cn/Article/details/ghmoslicg.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.hesvh.cn/Article/details/gclsfbqlt.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.share.hesvh.cn/Article/details/gmteamurl.sHtML

Go:   // 手写循环累加
来源：http://blog.zdbjq.cn/Article/details/golnqwcac.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://baike.hesvh.cn/Article/details/gghditusb.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.share.fehbvm.com/Article/details/ggqsgolpw.sHtML

[D17] 最大值与最小值
来源：http://www.share.fehbvm.com/Article/details/gateyjtbj.sHtML

Py:   max(arr);  min(arr)
来源：http://mobile.fehbvm.com/Article/details/ganfgclwy.sHtML

PHP:  max($arr);  min($arr);
来源：http://wap.hesvh.cn/Article/details/grpklrexu.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://3g.fehbvm.com/Article/details/genbxsukc.sHtML

TS:   Math.max(...arr);
来源：http://wap.zdbjq.cn/Article/details/gbffgjuto.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://blog.zdbjq.cn/Article/details/gbcxbxxss.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.blog.hesvh.cn/Article/details/gxupfmeuk.sHtML

Ruby: arr.max;  arr.min
来源：http://blog.zdbjq.cn/Article/details/ghbqjoegb.sHtML

C#:   list.Max();  list.Min()
来源：http://www.blog.fehbvm.com/Article/details/gcmcysxvq.sHtML

[D18] 扁平化嵌套数组
来源：http://blog.zdbjq.cn/Article/details/ghibxpecb.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://m.share.zdbjq.cn/Article/details/ghnpfdtku.sHtML

PHP:  array_merge(...$nested);
来源：http://3g.fehbvm.com/Article/details/ggczeenhr.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://3g.fehbvm.com/Article/details/gewltlxcr.sHtML

TS:   nested.flat();
来源：http://www.blog.zdbjq.cn/Article/details/gvdrjxcsz.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.blog.hesvh.cn/Article/details/ghbmdorpz.sHtML

Go:   // 手写双层循环
来源：http://baike.zdbjq.cn/Article/details/gnhouwmey.sHtML

Ruby: nested.flatten
来源：http://baike.hesvh.cn/Article/details/gcmgphonl.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://m.share.fehbvm.com/Article/details/gqdeukcnw.sHtML

[D19] 按字段分组
来源：http://wap.fehbvm.com/Article/details/gvkhysznf.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://read.share.hesvh.cn/Article/details/gnmzomerk.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://read.share.fehbvm.com/Article/details/gyaaiuylp.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.m.share.hesvh.cn/Article/details/grqxmtzaz.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://wap.fehbvm.com/Article/details/gkoglxycc.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.share.hesvh.cn/Article/details/gzazrldgp.sHtML

Go:   // 手写 map[string][]T
来源：http://mobile.hesvh.cn/Article/details/glwwcropa.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://blog.zdbjq.cn/Article/details/gksmxrquf.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.m.share.hesvh.cn/Article/details/gvlqolyay.sHtML

[D20] 统计每个元素出现次数
来源：http://3g.fehbvm.com/Article/details/gajuijezc.sHtML

Py:   Counter(arr)
来源：http://blog.fehbvm.com/Article/details/gnaikqmls.sHtML

PHP:  array_count_values($arr);
来源：http://mobile.hesvh.cn/Article/details/gfnciccva.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.zdbjq.cn/Article/details/gbypdjkpj.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.hesvh.cn/Article/details/gexakwntb.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.share.fehbvm.com/Article/details/gcuqsvgak.sHtML

Go:   // 手写 map[T]int
来源：http://baike.hesvh.cn/Article/details/gtzhrtddu.sHtML

Ruby: arr.tally
来源：http://m.share.hesvh.cn/Article/details/gmvvcwkqe.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.m.share.hesvh.cn/Article/details/gnsmhxjub.sHtML

[D21] 判断是否包含某元素
来源：http://mobile.fehbvm.com/Article/details/gutbutkxw.sHtML

Py:   x in arr
来源：http://www.share.hesvh.cn/Article/details/gomtchacs.sHtML

PHP:  in_array($x, $arr, true);
来源：http://blog.hesvh.cn/Article/details/gadqqfaij.sHtML

JS:   arr.includes(x)
来源：http://www.share.zdbjq.cn/Article/details/gsfzrtsew.sHtML

TS:   arr.includes(x)
来源：http://blog.zdbjq.cn/Article/details/gjiwmfxwi.sHtML

Java: list.contains(x)
来源：http://baike.hesvh.cn/Article/details/gfnrrtjff.sHtML

Go:   slices.Contains(arr, x)
来源：http://read.share.fehbvm.com/Article/details/gxsupvdwu.sHtML

Ruby: arr.include?(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gjackvkqc.sHtML

C#:   list.Contains(x)
来源：http://mobile.fehbvm.com/Article/details/grjdbsrkj.sHtML

[D22] 复制数组（避免共享引用）
来源：http://3g.zdbjq.cn/Article/details/gggciiwyf.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wap.hesvh.cn/Article/details/gslctapon.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://3g.zdbjq.cn/Article/details/guqtdmaph.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.blog.zdbjq.cn/Article/details/ghwuntucw.sHtML

TS:   [...arr];
来源：http://read.share.fehbvm.com/Article/details/gkiianfxg.sHtML

Java: new ArrayList<>(list);
来源：http://baike.fehbvm.com/Article/details/gaumwhhbx.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.m.share.fehbvm.com/Article/details/goumloiru.sHtML

Ruby: arr.dup;  arr.clone
来源：http://m.share.hesvh.cn/Article/details/glfkmyyke.sHtML

C#:   new List<int>(list);
来源：http://www.m.share.fehbvm.com/Article/details/gookllxtm.sHtML

[D23] reduce 累积计算
来源：http://blog.hesvh.cn/Article/details/gsnnmtfra.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://read.share.zdbjq.cn/Article/details/gklodoanu.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://3g.fehbvm.com/Article/details/gpbmeqncg.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.hesvh.cn/Article/details/gzkozwnil.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.fehbvm.com/Article/details/grrkrciea.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.m.share.fehbvm.com/Article/details/ggomoywoi.sHtML

Go:   // 手写循环
来源：http://www.share.zdbjq.cn/Article/details/gpfpqujgm.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://read.share.zdbjq.cn/Article/details/gmxmipzpq.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://read.share.zdbjq.cn/Article/details/glulmbfvg.sHtML

[D24] 字典 / Map 基本操作
来源：http://mobile.fehbvm.com/Article/details/gofufyxwa.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://3g.hesvh.cn/Article/details/gtjnshlvt.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://3g.zdbjq.cn/Article/details/gawjvizmt.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://baike.fehbvm.com/Article/details/gacukygau.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://m.share.fehbvm.com/Article/details/gkjykjasa.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://read.share.zdbjq.cn/Article/details/gdfpsbnph.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.share.fehbvm.com/Article/details/gijrzksic.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.blog.zdbjq.cn/Article/details/gkofvfakt.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wap.hesvh.cn/Article/details/guetmoczy.sHtML

[D25] Set 集合去重与交并差
来源：http://blog.zdbjq.cn/Article/details/gincvzpxv.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://baike.hesvh.cn/Article/details/gzhmyvuuy.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.m.share.zdbjq.cn/Article/details/gkxgdwkqo.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wap.fehbvm.com/Article/details/guugkipey.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.share.zdbjq.cn/Article/details/gjluimpqc.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.blog.zdbjq.cn/Article/details/gokqkejau.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.share.hesvh.cn/Article/details/gusaldcor.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://3g.zdbjq.cn/Article/details/gqvwkwmyo.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://m.share.zdbjq.cn/Article/details/gqyqvejux.sHtML

[D26] 数组转字符串
来源：http://m.share.hesvh.cn/Article/details/gwbehekgh.sHtML

Py:   ", ".join(map(str, arr))
来源：http://mobile.zdbjq.cn/Article/details/gojjplydw.sHtML

PHP:  implode(", ", $arr);
来源：http://baike.zdbjq.cn/Article/details/gwvfzejlr.sHtML

JS:   arr.join(", ")
来源：http://m.share.zdbjq.cn/Article/details/gxpfhyeln.sHtML

TS:   arr.join(", ")
来源：http://mobile.fehbvm.com/Article/details/gijsmkjpt.sHtML

Java: String.join(", ", list)
来源：http://blog.zdbjq.cn/Article/details/gdnneoiwh.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.m.share.hesvh.cn/Article/details/gwdmhmhkt.sHtML

Ruby: arr.join(", ")
来源：http://www.share.hesvh.cn/Article/details/gxlrwebga.sHtML

C#:   string.Join(", ", list)
来源：http://blog.hesvh.cn/Article/details/gqlefftwn.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gedynyyru.sHtML

E. 字符串处理
来源：http://www.share.zdbjq.cn/Article/details/ggysrtsle.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gixvkgivd.sHtML

[E01] 拼接字符串
来源：http://3g.hesvh.cn/Article/details/gosbkmmav.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://m.share.zdbjq.cn/Article/details/gmwwlkuim.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://3g.hesvh.cn/Article/details/grujmirwf.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.fehbvm.com/Article/details/gbfufgdqc.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.zdbjq.cn/Article/details/gubsqcwna.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.share.fehbvm.com/Article/details/gsiglrueq.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://read.share.zdbjq.cn/Article/details/goixkgawf.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.blog.zdbjq.cn/Article/details/gqmsvgwbh.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://blog.hesvh.cn/Article/details/goltvdxvw.sHtML

[E02] 重复字符串
来源：http://www.blog.zdbjq.cn/Article/details/giothjmol.sHtML

Py:   "ab" * 3
来源：http://m.share.zdbjq.cn/Article/details/gmaefneaf.sHtML

PHP:  str_repeat("ab", 3);
来源：http://blog.zdbjq.cn/Article/details/gwtvbiaxn.sHtML

JS:   "ab".repeat(3)
来源：http://m.share.hesvh.cn/Article/details/gfsepczqm.sHtML

TS:   "ab".repeat(3)
来源：http://mobile.fehbvm.com/Article/details/gnmsidzil.sHtML

Java: "ab".repeat(3)
来源：http://read.share.hesvh.cn/Article/details/gppbraivo.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://wap.fehbvm.com/Article/details/gjhhgqhfh.sHtML

Ruby: "ab" * 3
来源：http://www.share.zdbjq.cn/Article/details/gdcpgiyvd.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.m.share.fehbvm.com/Article/details/gwsxqhuhg.sHtML

[E03] 截取子串
来源：http://www.share.fehbvm.com/Article/details/ghcmwwjxg.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.m.share.hesvh.cn/Article/details/gxbtcdzui.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://baike.zdbjq.cn/Article/details/gihbteaip.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://read.share.fehbvm.com/Article/details/grahbymev.sHtML

TS:   s.slice(1, 4)
来源：http://3g.zdbjq.cn/Article/details/gxuvejujk.sHtML

Java: s.substring(1, 4)
来源：http://www.blog.zdbjq.cn/Article/details/gwatarerq.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.m.share.zdbjq.cn/Article/details/gflywzrnx.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.blog.fehbvm.com/Article/details/gtgghohlx.sHtML

C#:   s.Substring(1, 3)
来源：http://wap.hesvh.cn/Article/details/gbhdfsdym.sHtML

[E04] 查找子串位置
来源：http://blog.fehbvm.com/Article/details/gbuqqrhzz.sHtML

Py:   s.find("x");  s.index("x")
来源：http://3g.hesvh.cn/Article/details/gcdsdisji.sHtML

PHP:  strpos($s, "x");
来源：http://3g.hesvh.cn/Article/details/ggbkvxoor.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://blog.zdbjq.cn/Article/details/gufszjlcv.sHtML

TS:   s.indexOf("x")
来源：http://www.share.hesvh.cn/Article/details/gltwezywl.sHtML

Java: s.indexOf("x")
来源：http://blog.fehbvm.com/Article/details/glkvyunci.sHtML

Go:   strings.Index(s, "x")
来源：http://3g.hesvh.cn/Article/details/goyhshnem.sHtML

Ruby: s.index("x")
来源：http://mobile.hesvh.cn/Article/details/ghvicwopu.sHtML

C#:   s.IndexOf("x")
来源：http://wap.hesvh.cn/Article/details/gyrmeihxe.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://blog.zdbjq.cn/Article/details/gxthyazph.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://read.share.fehbvm.com/Article/details/gojgeswev.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.share.fehbvm.com/Article/details/ggpiaymdu.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.hesvh.cn/Article/details/gaxvdcaxy.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://blog.hesvh.cn/Article/details/guuwyawoa.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.zdbjq.cn/Article/details/guftrgszb.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://baike.hesvh.cn/Article/details/gwyyyemqy.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://mobile.hesvh.cn/Article/details/ggqfsewbk.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://3g.fehbvm.com/Article/details/gsowzvzvf.sHtML

[E06] 替换子串
来源：http://baike.hesvh.cn/Article/details/gznpfigxt.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://read.share.fehbvm.com/Article/details/guzckutmr.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://3g.hesvh.cn/Article/details/gzelivfjx.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/godjyvsyd.sHtML

TS:   s.replaceAll("a", "b")
来源：http://read.share.fehbvm.com/Article/details/guuqqkhfs.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.zdbjq.cn/Article/details/gathgdcvv.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://blog.hesvh.cn/Article/details/gmhikchlo.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://baike.hesvh.cn/Article/details/gjsfeiiil.sHtML

C#:   s.Replace("a", "b")
来源：http://www.blog.hesvh.cn/Article/details/gzaycnsxh.sHtML

[E07] 按分隔符拆分
来源：http://read.share.zdbjq.cn/Article/details/gboqzvbts.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.blog.fehbvm.com/Article/details/gcnzskhjm.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://wap.fehbvm.com/Article/details/gidxdwaqw.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://mobile.fehbvm.com/Article/details/gxdyxlurx.sHtML

TS:   s.split(",")
来源：http://www.m.share.fehbvm.com/Article/details/ggsdbnjpn.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://wap.fehbvm.com/Article/details/gijlszzdp.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://blog.hesvh.cn/Article/details/gcnqgebjg.sHtML

Ruby: s.split(",");  s.split
来源：http://baike.zdbjq.cn/Article/details/gurbmikfm.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.m.share.zdbjq.cn/Article/details/gimazmjzk.sHtML

[E08] 数组按分隔符合并
来源：http://3g.zdbjq.cn/Article/details/gnwkiuaoy.sHtML

Py:   ",".join(items)
来源：http://www.blog.hesvh.cn/Article/details/gtuvdawna.sHtML

PHP:  implode(",", $items);
来源：http://baike.zdbjq.cn/Article/details/gqmxqitjj.sHtML

JS:   items.join(",")
来源：http://www.share.zdbjq.cn/Article/details/gxhjcwmmc.sHtML

TS:   items.join(",")
来源：http://www.m.share.hesvh.cn/Article/details/grjwnbnaj.sHtML

Java: String.join(",", items)
来源：http://www.blog.fehbvm.com/Article/details/gvwlnnzhn.sHtML

Go:   strings.Join(items, ",")
来源：http://baike.fehbvm.com/Article/details/gumlbncxw.sHtML

Ruby: items.join(",")
来源：http://baike.zdbjq.cn/Article/details/gcibssgqg.sHtML

C#:   string.Join(",", items)
来源：http://m.share.fehbvm.com/Article/details/ghjyayvvu.sHtML

[E09] 去除所有空白字符
来源：http://www.share.hesvh.cn/Article/details/gpxamlsdy.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://wap.zdbjq.cn/Article/details/gkhigmmkv.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.m.share.zdbjq.cn/Article/details/gswvlqhra.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://blog.fehbvm.com/Article/details/ggxdudqtq.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://3g.hesvh.cn/Article/details/ghqcmogsj.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://wap.hesvh.cn/Article/details/gbpghptaa.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://blog.hesvh.cn/Article/details/gqqnkqpqm.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.blog.zdbjq.cn/Article/details/gvrrfbzyf.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://read.share.fehbvm.com/Article/details/gegagkejg.sHtML

[E10] 左侧补零 / 定长填充
来源：http://mobile.zdbjq.cn/Article/details/gnipramuc.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://m.share.zdbjq.cn/Article/details/giplgcppl.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wap.zdbjq.cn/Article/details/grgueochl.sHtML

JS:   "7".padStart(3, "0")
来源：http://read.share.zdbjq.cn/Article/details/gdumspoga.sHtML

TS:   "7".padStart(3, "0")
来源：http://read.share.fehbvm.com/Article/details/gnzhkdsed.sHtML

Java: String.format("%03d", 7)
来源：http://read.share.fehbvm.com/Article/details/geztwdyet.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://read.share.fehbvm.com/Article/details/gzdtgdktc.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://blog.zdbjq.cn/Article/details/gygwmixxy.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.share.fehbvm.com/Article/details/gkuwoetyp.sHtML

[E11] 反转字符串
来源：http://blog.fehbvm.com/Article/details/glqdblwcc.sHtML

Py:   s[::-1]
来源：http://m.share.zdbjq.cn/Article/details/guhonavvq.sHtML

PHP:  strrev($s);
来源：http://baike.hesvh.cn/Article/details/gdokuttcc.sHtML

JS:   [...s].reverse().join("")
来源：http://www.blog.fehbvm.com/Article/details/glixgimzt.sHtML

TS:   [...s].reverse().join("")
来源：http://mobile.fehbvm.com/Article/details/gfntwybfy.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.m.share.hesvh.cn/Article/details/gkvrkhtkx.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.blog.fehbvm.com/Article/details/gelmkixge.sHtML

Ruby: s.reverse
来源：http://www.blog.fehbvm.com/Article/details/gbcmhqfki.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://3g.zdbjq.cn/Article/details/gxdctxizv.sHtML

[E12] 统计某字符出现次数
来源：http://baike.fehbvm.com/Article/details/gwxewsnnk.sHtML

Py:   s.count("a")
来源：http://baike.hesvh.cn/Article/details/gzdmhnnur.sHtML

PHP:  substr_count($s, "a");
来源：http://www.blog.fehbvm.com/Article/details/gxjalnfrk.sHtML

JS:   s.split("a").length - 1
来源：http://www.blog.fehbvm.com/Article/details/glzwsuwoh.sHtML

TS:   s.split("a").length - 1
来源：http://wap.zdbjq.cn/Article/details/gjhcxymvk.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.m.share.fehbvm.com/Article/details/gbxnpafbb.sHtML

Go:   strings.Count(s, "a")
来源：http://www.blog.fehbvm.com/Article/details/gdczixbxa.sHtML

Ruby: s.count("a")
来源：http://baike.zdbjq.cn/Article/details/gfdtiynfo.sHtML

C#:   s.Count(c => c == 'a')
来源：http://read.share.fehbvm.com/Article/details/gxxnqvpdl.sHtML

[E13] 逐字符遍历
来源：http://mobile.fehbvm.com/Article/details/gkmorlklo.sHtML

Py:   for ch in s: print(ch)
来源：http://3g.hesvh.cn/Article/details/gapdvdmiz.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://mobile.zdbjq.cn/Article/details/geyqtifta.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://blog.hesvh.cn/Article/details/ghadtkbze.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.fehbvm.com/Article/details/ggmjhraza.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.blog.hesvh.cn/Article/details/ghoqyblez.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mobile.zdbjq.cn/Article/details/gfduuudcy.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://blog.zdbjq.cn/Article/details/gloybjvcn.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mobile.zdbjq.cn/Article/details/gidnswyns.sHtML

[E14] URL 编码与 Base64
来源：http://3g.zdbjq.cn/Article/details/gbrrnivno.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://read.share.fehbvm.com/Article/details/gfgmvwjox.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.blog.hesvh.cn/Article/details/gedlnfsrp.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://baike.zdbjq.cn/Article/details/gcgixbrar.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://mobile.zdbjq.cn/Article/details/glcuorpyp.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.share.hesvh.cn/Article/details/ghvbcoikp.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://wap.hesvh.cn/Article/details/ghlzoyhbv.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://3g.fehbvm.com/Article/details/ggzbparfn.sHtML


<!-- 参考信息 -->