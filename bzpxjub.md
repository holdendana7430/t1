代发 wailian999

Py:   len(arr)
来源：http://blog.zdbjq.cn/Article/details/gsoafragz.sHtML

PHP:  count($arr);
来源：http://read.share.hesvh.cn/Article/details/gacfpwzxm.sHtML

JS:   arr.length
来源：http://baike.hesvh.cn/Article/details/gqizcwsnn.sHtML

TS:   arr.length
来源：http://3g.fehbvm.com/Article/details/gtngvxbdy.sHtML

Java: list.size();
来源：http://mobile.zdbjq.cn/Article/details/grtgfbpmt.sHtML

Go:   len(arr)
来源：http://www.share.fehbvm.com/Article/details/grtkpbfbj.sHtML

Ruby: arr.length; arr.size
来源：http://www.blog.zdbjq.cn/Article/details/gfjrrexoe.sHtML

C#:   list.Count;
来源：http://www.m.share.zdbjq.cn/Article/details/gstshqnns.sHtML

[D07] 切片 / 取子数组
来源：http://wap.zdbjq.cn/Article/details/gmknongyg.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.share.zdbjq.cn/Article/details/gqckyrlui.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.m.share.fehbvm.com/Article/details/gskoxwfux.sHtML

JS:   arr.slice(1, 4);
来源：http://www.blog.hesvh.cn/Article/details/gbmlrkjji.sHtML

TS:   arr.slice(1, 4);
来源：http://www.blog.fehbvm.com/Article/details/ggziddthi.sHtML

Java: list.subList(1, 4);
来源：http://mobile.zdbjq.cn/Article/details/gcyyhrghy.sHtML

Go:   arr[1:4]
来源：http://wap.hesvh.cn/Article/details/gimbtgccu.sHtML

Ruby: arr[1, 3]
来源：http://www.blog.fehbvm.com/Article/details/gjsadoutb.sHtML

C#:   list.GetRange(1, 3);
来源：http://3g.hesvh.cn/Article/details/gvuqixnwr.sHtML

[D08] 合并两个数组
来源：http://mobile.hesvh.cn/Article/details/gwddvohep.sHtML

Py:   a + b;  a.extend(b)
来源：http://blog.hesvh.cn/Article/details/gjztdsshn.sHtML

PHP:  array_merge($a, $b);
来源：http://blog.fehbvm.com/Article/details/ghludovtc.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.m.share.zdbjq.cn/Article/details/gtdwjdjjk.sHtML

TS:   [...a, ...b];
来源：http://www.share.hesvh.cn/Article/details/gjzscxaht.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.blog.hesvh.cn/Article/details/grmlogrew.sHtML

Go:   append(a, b...)
来源：http://mobile.hesvh.cn/Article/details/gpomsepii.sHtML

Ruby: a + b;  a.concat(b)
来源：http://m.share.hesvh.cn/Article/details/gepgkeabx.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.blog.hesvh.cn/Article/details/gknnoikqx.sHtML

[D09] 排序（升序）
来源：http://www.m.share.zdbjq.cn/Article/details/gphdilbvz.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.hesvh.cn/Article/details/gtzegsvwx.sHtML

PHP:  sort($arr);
来源：http://read.share.fehbvm.com/Article/details/gplwfkfop.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.m.share.zdbjq.cn/Article/details/gddsghnno.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://wap.zdbjq.cn/Article/details/gmxaufrfn.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://blog.fehbvm.com/Article/details/gdujfcemw.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://wap.zdbjq.cn/Article/details/gurexiluk.sHtML

Ruby: arr.sort
来源：http://www.share.zdbjq.cn/Article/details/ggzzqggsp.sHtML

C#:   list.Sort();
来源：http://m.share.fehbvm.com/Article/details/gbrfnjljh.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://wap.fehbvm.com/Article/details/gqudfomel.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://3g.fehbvm.com/Article/details/gxwqvlfwn.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.hesvh.cn/Article/details/gwpyfwmfp.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.zdbjq.cn/Article/details/gldxjuwel.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.hesvh.cn/Article/details/gdadpwlbk.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.share.zdbjq.cn/Article/details/gtvrmablp.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://m.share.hesvh.cn/Article/details/ghsaduugc.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.share.hesvh.cn/Article/details/glgwwsrdk.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://m.share.fehbvm.com/Article/details/ganlzypwh.sHtML

[D11] 反转数组
来源：http://www.blog.fehbvm.com/Article/details/ggccznvsw.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://mobile.zdbjq.cn/Article/details/gtenrgrib.sHtML

PHP:  array_reverse($arr);
来源：http://www.m.share.hesvh.cn/Article/details/gpjwkmhfp.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://read.share.hesvh.cn/Article/details/gnykdanzs.sHtML

TS:   [...arr].reverse();
来源：http://mobile.zdbjq.cn/Article/details/gjsjnjmot.sHtML

Java: Collections.reverse(list);
来源：http://mobile.hesvh.cn/Article/details/gafxzhonl.sHtML

Go:   slices.Reverse(arr)
来源：http://www.blog.fehbvm.com/Article/details/gtsxcldgw.sHtML

Ruby: arr.reverse
来源：http://mobile.zdbjq.cn/Article/details/gmuxijxdv.sHtML

C#:   list.Reverse();
来源：http://wap.fehbvm.com/Article/details/ghajglaqj.sHtML

[D12] 查找元素下标
来源：http://mobile.fehbvm.com/Article/details/gsfoadphp.sHtML

Py:   arr.index(x);  x in arr
来源：http://baike.hesvh.cn/Article/details/glkqnedrk.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://read.share.hesvh.cn/Article/details/gcnnzvzqt.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.zdbjq.cn/Article/details/ggbimvrky.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.zdbjq.cn/Article/details/gbnzmifyg.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://m.share.zdbjq.cn/Article/details/gtgilddih.sHtML

Go:   slices.Index(arr, x)
来源：http://www.m.share.hesvh.cn/Article/details/gqgwbjpmn.sHtML

Ruby: arr.index(x)
来源：http://www.share.zdbjq.cn/Article/details/gdmqfyyfe.sHtML

C#:   list.IndexOf(x);
来源：http://baike.zdbjq.cn/Article/details/grnonlseb.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.share.hesvh.cn/Article/details/ggikrgqcl.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://wap.fehbvm.com/Article/details/gbdoylduo.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://read.share.fehbvm.com/Article/details/gjuiinrrc.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.m.share.zdbjq.cn/Article/details/gwwowtbku.sHtML

TS:   arr.filter(x => x > 3)
来源：http://mobile.zdbjq.cn/Article/details/gdnuknaus.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://baike.fehbvm.com/Article/details/gegjahfzf.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://m.share.zdbjq.cn/Article/details/gjymliuym.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://read.share.hesvh.cn/Article/details/gtkvaqidp.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.blog.hesvh.cn/Article/details/gjtxzkili.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.blog.hesvh.cn/Article/details/gyqbxlnvk.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://read.share.hesvh.cn/Article/details/geuwrhavv.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://m.share.hesvh.cn/Article/details/gtisgxajo.sHtML

JS:   arr.map(x => x * 2)
来源：http://baike.fehbvm.com/Article/details/gtyrkxspd.sHtML

TS:   arr.map(x => x * 2)
来源：http://mobile.hesvh.cn/Article/details/gsqweelki.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://mobile.fehbvm.com/Article/details/gpxfucnnh.sHtML

Go:   // 手写循环
来源：http://blog.zdbjq.cn/Article/details/gqnexynpq.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.share.fehbvm.com/Article/details/godurkgjp.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://blog.fehbvm.com/Article/details/gdszqzsvs.sHtML

[D15] 去重
来源：http://www.m.share.zdbjq.cn/Article/details/guslfewbb.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.blog.hesvh.cn/Article/details/gegeyyfpq.sHtML

PHP:  array_unique($arr);
来源：http://read.share.hesvh.cn/Article/details/ghynwcjpq.sHtML

JS:   [...new Set(arr)]
来源：http://m.share.hesvh.cn/Article/details/gekbgdxkw.sHtML

TS:   [...new Set(arr)]
来源：http://baike.fehbvm.com/Article/details/giuusrfsz.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://m.share.hesvh.cn/Article/details/giqhyuwvg.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://m.share.hesvh.cn/Article/details/gxzhqkdcp.sHtML

Ruby: arr.uniq
来源：http://read.share.zdbjq.cn/Article/details/gdknostss.sHtML

C#:   list.Distinct().ToList()
来源：http://baike.zdbjq.cn/Article/details/gdktxuxfm.sHtML

[D16] 求和与平均值
来源：http://m.share.hesvh.cn/Article/details/gycvneocu.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wap.zdbjq.cn/Article/details/gdcldpqmg.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.share.zdbjq.cn/Article/details/ggjpppbfr.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.hesvh.cn/Article/details/gkuauwihm.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.fehbvm.com/Article/details/gnnqkskfv.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://baike.hesvh.cn/Article/details/grbyrrfyl.sHtML

Go:   // 手写循环累加
来源：http://m.share.fehbvm.com/Article/details/ggtsdbjmr.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.share.fehbvm.com/Article/details/gdhmackmm.sHtML

C#:   list.Sum();  list.Average()
来源：http://m.share.zdbjq.cn/Article/details/giienqddl.sHtML

[D17] 最大值与最小值
来源：http://3g.fehbvm.com/Article/details/guvjvhkwe.sHtML

Py:   max(arr);  min(arr)
来源：http://3g.zdbjq.cn/Article/details/gltjychwj.sHtML

PHP:  max($arr);  min($arr);
来源：http://wap.hesvh.cn/Article/details/gblbkizwp.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://3g.zdbjq.cn/Article/details/goctxntlv.sHtML

TS:   Math.max(...arr);
来源：http://www.share.fehbvm.com/Article/details/gmswlofda.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.m.share.fehbvm.com/Article/details/gdykgldjl.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://m.share.fehbvm.com/Article/details/gzmpspvsg.sHtML

Ruby: arr.max;  arr.min
来源：http://mobile.hesvh.cn/Article/details/gtgrkgbsc.sHtML

C#:   list.Max();  list.Min()
来源：http://baike.zdbjq.cn/Article/details/gdklttzlu.sHtML

[D18] 扁平化嵌套数组
来源：http://3g.fehbvm.com/Article/details/gohfagqpt.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://m.share.fehbvm.com/Article/details/gprfvuimi.sHtML

PHP:  array_merge(...$nested);
来源：http://m.share.hesvh.cn/Article/details/gyxokmbai.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://3g.zdbjq.cn/Article/details/gejnxlolo.sHtML

TS:   nested.flat();
来源：http://m.share.fehbvm.com/Article/details/gcklrmoyu.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://blog.hesvh.cn/Article/details/gietxigzl.sHtML

Go:   // 手写双层循环
来源：http://read.share.hesvh.cn/Article/details/gvspnuqza.sHtML

Ruby: nested.flatten
来源：http://3g.fehbvm.com/Article/details/gxyngpcid.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.m.share.hesvh.cn/Article/details/gvazgrfdg.sHtML

[D19] 按字段分组
来源：http://3g.hesvh.cn/Article/details/ghfqqeegm.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://m.share.hesvh.cn/Article/details/gmkvccarx.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://read.share.fehbvm.com/Article/details/gxwndyfnx.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://3g.hesvh.cn/Article/details/gihmvzjti.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://3g.fehbvm.com/Article/details/gmjrubdfh.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://m.share.hesvh.cn/Article/details/gcfreppua.sHtML

Go:   // 手写 map[string][]T
来源：http://www.blog.zdbjq.cn/Article/details/ghknybhbe.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.m.share.hesvh.cn/Article/details/gipscpcdg.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://3g.fehbvm.com/Article/details/gwruxvyls.sHtML

[D20] 统计每个元素出现次数
来源：http://3g.hesvh.cn/Article/details/gxuzjvjpq.sHtML

Py:   Counter(arr)
来源：http://baike.zdbjq.cn/Article/details/gozedqrri.sHtML

PHP:  array_count_values($arr);
来源：http://www.m.share.hesvh.cn/Article/details/gmlvntmgp.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.hesvh.cn/Article/details/gjvkzqnur.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.hesvh.cn/Article/details/gsbhcoysv.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://baike.hesvh.cn/Article/details/gxrzfrwjg.sHtML

Go:   // 手写 map[T]int
来源：http://www.share.hesvh.cn/Article/details/gfvxpghmu.sHtML

Ruby: arr.tally
来源：http://www.blog.zdbjq.cn/Article/details/gxrivriya.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://m.share.hesvh.cn/Article/details/giltwfdyt.sHtML

[D21] 判断是否包含某元素
来源：http://blog.hesvh.cn/Article/details/gfhtkfica.sHtML

Py:   x in arr
来源：http://wap.zdbjq.cn/Article/details/ghsloljhr.sHtML

PHP:  in_array($x, $arr, true);
来源：http://m.share.fehbvm.com/Article/details/gfmsmyebz.sHtML

JS:   arr.includes(x)
来源：http://www.m.share.hesvh.cn/Article/details/gkwjwmkuj.sHtML

TS:   arr.includes(x)
来源：http://wap.zdbjq.cn/Article/details/gqmomcifb.sHtML

Java: list.contains(x)
来源：http://wap.hesvh.cn/Article/details/gyuuhccft.sHtML

Go:   slices.Contains(arr, x)
来源：http://mobile.fehbvm.com/Article/details/ghxhfsdwd.sHtML

Ruby: arr.include?(x)
来源：http://baike.hesvh.cn/Article/details/gzhjjpxes.sHtML

C#:   list.Contains(x)
来源：http://www.m.share.hesvh.cn/Article/details/gudbfrlng.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.m.share.fehbvm.com/Article/details/gomvdfqej.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://blog.fehbvm.com/Article/details/gmwnjugpt.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://read.share.hesvh.cn/Article/details/gpbelujld.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gopkxdncp.sHtML

TS:   [...arr];
来源：http://3g.hesvh.cn/Article/details/gvtfzzcro.sHtML

Java: new ArrayList<>(list);
来源：http://read.share.zdbjq.cn/Article/details/gpfofudtk.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.blog.hesvh.cn/Article/details/gszvcmsfy.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.share.fehbvm.com/Article/details/ghhsdqolk.sHtML

C#:   new List<int>(list);
来源：http://www.share.zdbjq.cn/Article/details/gfkswzgha.sHtML

[D23] reduce 累积计算
来源：http://wap.zdbjq.cn/Article/details/gjmhjqzps.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.m.share.fehbvm.com/Article/details/gesffhdut.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://m.share.zdbjq.cn/Article/details/gneffyxem.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.zdbjq.cn/Article/details/gopqczyrn.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.fehbvm.com/Article/details/ggfiofuam.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.share.fehbvm.com/Article/details/gdyjjybvp.sHtML

Go:   // 手写循环
来源：http://blog.zdbjq.cn/Article/details/gzxcelnnm.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://blog.hesvh.cn/Article/details/glkroqmvi.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://m.share.zdbjq.cn/Article/details/giutzukga.sHtML

[D24] 字典 / Map 基本操作
来源：http://m.share.fehbvm.com/Article/details/gkomucliq.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://blog.fehbvm.com/Article/details/gjupxyxdy.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://3g.zdbjq.cn/Article/details/gdslseiwv.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://blog.hesvh.cn/Article/details/ghmzgcpab.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://mobile.fehbvm.com/Article/details/gjehcoqcb.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://read.share.fehbvm.com/Article/details/ggkxbcavz.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://read.share.hesvh.cn/Article/details/gxmzjwzry.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.share.hesvh.cn/Article/details/gtmccvowt.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.share.hesvh.cn/Article/details/gdigwvebn.sHtML

[D25] Set 集合去重与交并差
来源：http://www.share.fehbvm.com/Article/details/glligefte.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.m.share.hesvh.cn/Article/details/geaeepyto.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.blog.hesvh.cn/Article/details/gqrwkbqoq.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://m.share.fehbvm.com/Article/details/gutujbbfh.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.m.share.fehbvm.com/Article/details/ghvjtifgf.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://blog.zdbjq.cn/Article/details/gbkcazoyr.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.blog.hesvh.cn/Article/details/gnizclyjk.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mobile.fehbvm.com/Article/details/gnjlzcict.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://baike.hesvh.cn/Article/details/ggsapiidb.sHtML

[D26] 数组转字符串
来源：http://baike.fehbvm.com/Article/details/gjzephrnr.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.m.share.fehbvm.com/Article/details/gmwmalwzg.sHtML

PHP:  implode(", ", $arr);
来源：http://www.share.fehbvm.com/Article/details/gwmwprhxy.sHtML

JS:   arr.join(", ")
来源：http://www.m.share.fehbvm.com/Article/details/ggdpmtfxm.sHtML

TS:   arr.join(", ")
来源：http://www.blog.zdbjq.cn/Article/details/gmtlbzjas.sHtML

Java: String.join(", ", list)
来源：http://3g.zdbjq.cn/Article/details/grrvmboly.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.share.zdbjq.cn/Article/details/gjymeqbtv.sHtML

Ruby: arr.join(", ")
来源：http://baike.hesvh.cn/Article/details/gxgqbsahh.sHtML

C#:   string.Join(", ", list)
来源：http://www.m.share.fehbvm.com/Article/details/gkxritcmp.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gbicvhpnq.sHtML

E. 字符串处理
来源：http://www.blog.zdbjq.cn/Article/details/gvltilyub.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/goqeyxwhe.sHtML

[E01] 拼接字符串
来源：http://3g.zdbjq.cn/Article/details/gqbexyids.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://3g.fehbvm.com/Article/details/glsulyjmw.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://blog.fehbvm.com/Article/details/gomopuoqq.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.hesvh.cn/Article/details/gdamdhsvw.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.fehbvm.com/Article/details/glvnviwnm.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://blog.fehbvm.com/Article/details/ghjpfdgll.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wap.hesvh.cn/Article/details/gicizinpm.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://baike.fehbvm.com/Article/details/gieizjiqn.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://m.share.fehbvm.com/Article/details/geiisoeil.sHtML

[E02] 重复字符串
来源：http://www.share.fehbvm.com/Article/details/gzrdvqmhd.sHtML

Py:   "ab" * 3
来源：http://www.blog.fehbvm.com/Article/details/gnznwrijl.sHtML

PHP:  str_repeat("ab", 3);
来源：http://read.share.fehbvm.com/Article/details/gizrfxjsh.sHtML

JS:   "ab".repeat(3)
来源：http://www.blog.zdbjq.cn/Article/details/ghcqqvlav.sHtML

TS:   "ab".repeat(3)
来源：http://wap.hesvh.cn/Article/details/gzwdikiun.sHtML

Java: "ab".repeat(3)
来源：http://3g.fehbvm.com/Article/details/gekzdwpga.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.blog.hesvh.cn/Article/details/ggmigiyyq.sHtML

Ruby: "ab" * 3
来源：http://www.m.share.fehbvm.com/Article/details/gruxyeaos.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://m.share.hesvh.cn/Article/details/gdvfqwqdm.sHtML

[E03] 截取子串
来源：http://www.share.zdbjq.cn/Article/details/gwgczeijp.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://baike.fehbvm.com/Article/details/giaooaogb.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.m.share.fehbvm.com/Article/details/glgmrvwmv.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.share.fehbvm.com/Article/details/gtvyftvet.sHtML

TS:   s.slice(1, 4)
来源：http://www.blog.fehbvm.com/Article/details/gzhglrsei.sHtML

Java: s.substring(1, 4)
来源：http://3g.zdbjq.cn/Article/details/gnvzhuwar.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://mobile.hesvh.cn/Article/details/gwzwretgr.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.blog.hesvh.cn/Article/details/gooiaugrw.sHtML

C#:   s.Substring(1, 3)
来源：http://m.share.zdbjq.cn/Article/details/gpooslbao.sHtML

[E04] 查找子串位置
来源：http://baike.hesvh.cn/Article/details/gymzofiua.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.blog.fehbvm.com/Article/details/guubkqirt.sHtML

PHP:  strpos($s, "x");
来源：http://3g.fehbvm.com/Article/details/giiirmbrv.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://3g.fehbvm.com/Article/details/gzpzupnjm.sHtML

TS:   s.indexOf("x")
来源：http://blog.fehbvm.com/Article/details/gxjhxnxyu.sHtML

Java: s.indexOf("x")
来源：http://m.share.zdbjq.cn/Article/details/gddvqfhed.sHtML

Go:   strings.Index(s, "x")
来源：http://m.share.fehbvm.com/Article/details/gwjautdtu.sHtML

Ruby: s.index("x")
来源：http://www.m.share.zdbjq.cn/Article/details/gwxwnfzqw.sHtML

C#:   s.IndexOf("x")
来源：http://read.share.zdbjq.cn/Article/details/gblzkaxnz.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://m.share.zdbjq.cn/Article/details/gpxezxkps.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://read.share.zdbjq.cn/Article/details/ghisejdsi.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://baike.fehbvm.com/Article/details/gfemadera.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.fehbvm.com/Article/details/gtelfehie.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.m.share.zdbjq.cn/Article/details/gsmeywfsu.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.fehbvm.com/Article/details/gheffgyme.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wap.fehbvm.com/Article/details/gmwtrnhjd.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://blog.zdbjq.cn/Article/details/gifxnmpcr.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://blog.hesvh.cn/Article/details/gezljasmp.sHtML

[E06] 替换子串
来源：http://3g.zdbjq.cn/Article/details/gfiklpjvg.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://wap.zdbjq.cn/Article/details/gytikjyup.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://3g.zdbjq.cn/Article/details/gpuvjgctb.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.zdbjq.cn/Article/details/gomhjtmag.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/gmxurlhmv.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.hesvh.cn/Article/details/gfedcmcuz.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.blog.hesvh.cn/Article/details/gtpwuosdh.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/gefjmgeyq.sHtML

C#:   s.Replace("a", "b")
来源：http://blog.zdbjq.cn/Article/details/gokvqejvd.sHtML

[E07] 按分隔符拆分
来源：http://www.share.fehbvm.com/Article/details/gbjqmiepm.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://blog.fehbvm.com/Article/details/gjzhahork.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://blog.hesvh.cn/Article/details/glxdmctfl.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://read.share.fehbvm.com/Article/details/gntklobkd.sHtML

TS:   s.split(",")
来源：http://www.m.share.hesvh.cn/Article/details/gbvtunrjh.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://read.share.hesvh.cn/Article/details/gwyrccugj.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.blog.zdbjq.cn/Article/details/gemyhisnz.sHtML

Ruby: s.split(",");  s.split
来源：http://wap.zdbjq.cn/Article/details/gpbmkdgod.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wap.zdbjq.cn/Article/details/grdkmuldm.sHtML

[E08] 数组按分隔符合并
来源：http://www.m.share.zdbjq.cn/Article/details/gzahampat.sHtML

Py:   ",".join(items)
来源：http://m.share.zdbjq.cn/Article/details/ghlolxwux.sHtML

PHP:  implode(",", $items);
来源：http://blog.hesvh.cn/Article/details/gdlydgmhw.sHtML

JS:   items.join(",")
来源：http://www.blog.hesvh.cn/Article/details/gjcjolyrh.sHtML

TS:   items.join(",")
来源：http://www.blog.hesvh.cn/Article/details/gnlbwcvth.sHtML

Java: String.join(",", items)
来源：http://read.share.zdbjq.cn/Article/details/gthyvspph.sHtML

Go:   strings.Join(items, ",")
来源：http://blog.zdbjq.cn/Article/details/gadqdxynq.sHtML

Ruby: items.join(",")
来源：http://3g.zdbjq.cn/Article/details/gtuakixuo.sHtML

C#:   string.Join(",", items)
来源：http://baike.zdbjq.cn/Article/details/gyofenemd.sHtML

[E09] 去除所有空白字符
来源：http://baike.hesvh.cn/Article/details/gthtpkdpc.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://baike.fehbvm.com/Article/details/gjwmevsnf.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.share.fehbvm.com/Article/details/gfeeompmh.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://3g.hesvh.cn/Article/details/gpausbbrr.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://baike.fehbvm.com/Article/details/gfkpilbtp.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://3g.hesvh.cn/Article/details/gdpkryjcn.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.m.share.hesvh.cn/Article/details/glbexmxof.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://read.share.hesvh.cn/Article/details/gayedttha.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://blog.hesvh.cn/Article/details/ghfbtvywc.sHtML

[E10] 左侧补零 / 定长填充
来源：http://3g.zdbjq.cn/Article/details/gjitjttje.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.blog.zdbjq.cn/Article/details/gcsdgnwkv.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.m.share.hesvh.cn/Article/details/gdablpwso.sHtML

JS:   "7".padStart(3, "0")
来源：http://m.share.zdbjq.cn/Article/details/glqdwaxid.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.blog.zdbjq.cn/Article/details/gbvjzdqju.sHtML

Java: String.format("%03d", 7)
来源：http://baike.hesvh.cn/Article/details/gvbcxyljp.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.blog.zdbjq.cn/Article/details/gqqfkxqmj.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.blog.fehbvm.com/Article/details/gevvhiyat.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://mobile.fehbvm.com/Article/details/grtbfbejx.sHtML

[E11] 反转字符串
来源：http://3g.hesvh.cn/Article/details/gdkqetopp.sHtML

Py:   s[::-1]
来源：http://read.share.zdbjq.cn/Article/details/gzvovfugb.sHtML

PHP:  strrev($s);
来源：http://m.share.hesvh.cn/Article/details/gbdfouukr.sHtML

JS:   [...s].reverse().join("")
来源：http://baike.zdbjq.cn/Article/details/gimrhxtge.sHtML

TS:   [...s].reverse().join("")
来源：http://mobile.hesvh.cn/Article/details/gdgmjyotr.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.blog.zdbjq.cn/Article/details/ghfhhoocy.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://m.share.hesvh.cn/Article/details/gzfkgnygs.sHtML

Ruby: s.reverse
来源：http://blog.fehbvm.com/Article/details/gxwlmciea.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.blog.zdbjq.cn/Article/details/geluajpmc.sHtML

[E12] 统计某字符出现次数
来源：http://read.share.hesvh.cn/Article/details/gpbdvleuw.sHtML

Py:   s.count("a")
来源：http://www.m.share.fehbvm.com/Article/details/gauspywus.sHtML

PHP:  substr_count($s, "a");
来源：http://www.share.hesvh.cn/Article/details/gtwnfizzn.sHtML

JS:   s.split("a").length - 1
来源：http://www.m.share.hesvh.cn/Article/details/gxufmakwa.sHtML

TS:   s.split("a").length - 1
来源：http://baike.hesvh.cn/Article/details/gdagubxiq.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.m.share.fehbvm.com/Article/details/glykgmrxo.sHtML

Go:   strings.Count(s, "a")
来源：http://www.share.zdbjq.cn/Article/details/gcfrmikry.sHtML

Ruby: s.count("a")
来源：http://baike.zdbjq.cn/Article/details/gfhockjaf.sHtML

C#:   s.Count(c => c == 'a')
来源：http://blog.hesvh.cn/Article/details/grycbdzkc.sHtML

[E13] 逐字符遍历
来源：http://blog.zdbjq.cn/Article/details/gauftkkzb.sHtML


<!-- 参考信息 -->