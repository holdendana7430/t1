代发 wailian999

Go:   arr[0]; arr[0] = 9
来源：http://www.share.fehbvm.com/Article/details/ghbzvjwxz.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.fehbvm.com/Article/details/gulskpabi.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://blog.fehbvm.com/Article/details/gdwbyocbw.sHtML

[D06] 数组长度
来源：http://www.blog.hesvh.cn/Article/details/ganuyxldg.sHtML

Py:   len(arr)
来源：http://blog.fehbvm.com/Article/details/gvbwcatgn.sHtML

PHP:  count($arr);
来源：http://www.share.hesvh.cn/Article/details/gqysadmtm.sHtML

JS:   arr.length
来源：http://wap.hesvh.cn/Article/details/gmqgkecys.sHtML

TS:   arr.length
来源：http://3g.hesvh.cn/Article/details/gjbwutkbb.sHtML

Java: list.size();
来源：http://www.share.hesvh.cn/Article/details/glujjrnck.sHtML

Go:   len(arr)
来源：http://wap.fehbvm.com/Article/details/gqekhdgjw.sHtML

Ruby: arr.length; arr.size
来源：http://www.m.share.fehbvm.com/Article/details/gvlicuycq.sHtML

C#:   list.Count;
来源：http://3g.hesvh.cn/Article/details/gwrmwhvae.sHtML

[D07] 切片 / 取子数组
来源：http://www.blog.zdbjq.cn/Article/details/gsgjjjdzs.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.blog.hesvh.cn/Article/details/gedayamqs.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://blog.fehbvm.com/Article/details/gdijkxwtf.sHtML

JS:   arr.slice(1, 4);
来源：http://3g.zdbjq.cn/Article/details/geiivzdvi.sHtML

TS:   arr.slice(1, 4);
来源：http://www.share.hesvh.cn/Article/details/gcllxfbbs.sHtML

Java: list.subList(1, 4);
来源：http://mobile.zdbjq.cn/Article/details/ghcsviomn.sHtML

Go:   arr[1:4]
来源：http://m.share.hesvh.cn/Article/details/gepccnxcy.sHtML

Ruby: arr[1, 3]
来源：http://www.share.fehbvm.com/Article/details/gxyxfvdyv.sHtML

C#:   list.GetRange(1, 3);
来源：http://wap.fehbvm.com/Article/details/gjjzzcdew.sHtML

[D08] 合并两个数组
来源：http://baike.zdbjq.cn/Article/details/getvtgvae.sHtML

Py:   a + b;  a.extend(b)
来源：http://mobile.hesvh.cn/Article/details/gxqgzzafh.sHtML

PHP:  array_merge($a, $b);
来源：http://3g.zdbjq.cn/Article/details/gxsmqkvaq.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://3g.hesvh.cn/Article/details/gywvdwydf.sHtML

TS:   [...a, ...b];
来源：http://read.share.fehbvm.com/Article/details/gzshkqxbj.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://3g.fehbvm.com/Article/details/gytpfbwqz.sHtML

Go:   append(a, b...)
来源：http://blog.zdbjq.cn/Article/details/gewxhpnlt.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.m.share.hesvh.cn/Article/details/gpreunsmg.sHtML

C#:   a.Concat(b).ToList()
来源：http://m.share.hesvh.cn/Article/details/ggzikejvn.sHtML

[D09] 排序（升序）
来源：http://wap.hesvh.cn/Article/details/ghicifzou.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.fehbvm.com/Article/details/gkqskxrkb.sHtML

PHP:  sort($arr);
来源：http://3g.hesvh.cn/Article/details/gzhwlulpw.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://blog.zdbjq.cn/Article/details/gjwjljegw.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.blog.zdbjq.cn/Article/details/gsmjspuoo.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://blog.fehbvm.com/Article/details/grsojbmsd.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.share.fehbvm.com/Article/details/girskmuvi.sHtML

Ruby: arr.sort
来源：http://read.share.hesvh.cn/Article/details/gkimgheuw.sHtML

C#:   list.Sort();
来源：http://3g.fehbvm.com/Article/details/giuzquhgz.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://3g.hesvh.cn/Article/details/graickerr.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://blog.hesvh.cn/Article/details/gfituznur.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.fehbvm.com/Article/details/gpspdideh.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.zdbjq.cn/Article/details/gpjbsrrnl.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.fehbvm.com/Article/details/gngzeevqv.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://m.share.fehbvm.com/Article/details/gvgvgmnky.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wap.fehbvm.com/Article/details/gnlentlod.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://read.share.hesvh.cn/Article/details/gxtknndyp.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://m.share.fehbvm.com/Article/details/gmtkrbzwc.sHtML

[D11] 反转数组
来源：http://3g.fehbvm.com/Article/details/gwvlruxjd.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://baike.fehbvm.com/Article/details/gnxsgyvio.sHtML

PHP:  array_reverse($arr);
来源：http://www.blog.zdbjq.cn/Article/details/gtmzzksja.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.share.zdbjq.cn/Article/details/ghhskupai.sHtML

TS:   [...arr].reverse();
来源：http://baike.hesvh.cn/Article/details/ggexkuyeo.sHtML

Java: Collections.reverse(list);
来源：http://3g.hesvh.cn/Article/details/gojhxaxlh.sHtML

Go:   slices.Reverse(arr)
来源：http://mobile.hesvh.cn/Article/details/gtmdwhzkr.sHtML

Ruby: arr.reverse
来源：http://blog.fehbvm.com/Article/details/gnkyucchv.sHtML

C#:   list.Reverse();
来源：http://read.share.fehbvm.com/Article/details/gumcxejfz.sHtML

[D12] 查找元素下标
来源：http://wap.zdbjq.cn/Article/details/gjjbcxwrp.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.share.hesvh.cn/Article/details/gqzfgilcx.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://m.share.zdbjq.cn/Article/details/gskoljbun.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.zdbjq.cn/Article/details/gyghfmkwj.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.zdbjq.cn/Article/details/gfdgoztmu.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://m.share.zdbjq.cn/Article/details/gtcmvojvn.sHtML

Go:   slices.Index(arr, x)
来源：http://www.share.hesvh.cn/Article/details/ghkbpcutw.sHtML

Ruby: arr.index(x)
来源：http://blog.hesvh.cn/Article/details/gkxrxqtjc.sHtML

C#:   list.IndexOf(x);
来源：http://wap.hesvh.cn/Article/details/ggucbvevu.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.blog.fehbvm.com/Article/details/gdafeosjx.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://blog.zdbjq.cn/Article/details/gnvlqyrbw.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://blog.hesvh.cn/Article/details/gbzujizyg.sHtML

JS:   arr.filter(x => x > 3)
来源：http://read.share.hesvh.cn/Article/details/gkpifluft.sHtML

TS:   arr.filter(x => x > 3)
来源：http://wap.zdbjq.cn/Article/details/gnkglbsur.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://read.share.zdbjq.cn/Article/details/gdfihzupn.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mobile.fehbvm.com/Article/details/gevehszlm.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://read.share.fehbvm.com/Article/details/ghlbodkzc.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://wap.hesvh.cn/Article/details/gbmwxcxun.sHtML

[D14] 映射转换（每个元素变形）
来源：http://blog.zdbjq.cn/Article/details/ggwepugho.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mobile.fehbvm.com/Article/details/goskoxacm.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://baike.zdbjq.cn/Article/details/gmqftkdll.sHtML

JS:   arr.map(x => x * 2)
来源：http://wap.zdbjq.cn/Article/details/glkunvtvb.sHtML

TS:   arr.map(x => x * 2)
来源：http://wap.hesvh.cn/Article/details/gkzfhuyac.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://baike.zdbjq.cn/Article/details/gotfyqfik.sHtML

Go:   // 手写循环
来源：http://mobile.fehbvm.com/Article/details/gvranpaef.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://m.share.zdbjq.cn/Article/details/gxcwwigac.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://3g.hesvh.cn/Article/details/gfvxueanx.sHtML

[D15] 去重
来源：http://baike.zdbjq.cn/Article/details/gktogruxm.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.m.share.zdbjq.cn/Article/details/guhipwvoq.sHtML

PHP:  array_unique($arr);
来源：http://baike.fehbvm.com/Article/details/gptcbpdlv.sHtML

JS:   [...new Set(arr)]
来源：http://blog.fehbvm.com/Article/details/goocypwyl.sHtML

TS:   [...new Set(arr)]
来源：http://wap.fehbvm.com/Article/details/gsxsilmre.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://read.share.zdbjq.cn/Article/details/gskegpxay.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://wap.hesvh.cn/Article/details/gyjfuacxx.sHtML

Ruby: arr.uniq
来源：http://baike.fehbvm.com/Article/details/gpgxangsn.sHtML

C#:   list.Distinct().ToList()
来源：http://3g.zdbjq.cn/Article/details/gtsdgkivi.sHtML

[D16] 求和与平均值
来源：http://blog.zdbjq.cn/Article/details/gyzxjuobh.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://3g.hesvh.cn/Article/details/gvhcrqxcp.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.share.hesvh.cn/Article/details/goaiofell.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.zdbjq.cn/Article/details/gyajctlwh.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.hesvh.cn/Article/details/gypumpwnu.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://blog.zdbjq.cn/Article/details/gddcpypbh.sHtML

Go:   // 手写循环累加
来源：http://m.share.hesvh.cn/Article/details/gqsotbsep.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://read.share.fehbvm.com/Article/details/gerfppylv.sHtML

C#:   list.Sum();  list.Average()
来源：http://3g.hesvh.cn/Article/details/glygczqbs.sHtML

[D17] 最大值与最小值
来源：http://wap.zdbjq.cn/Article/details/gjsczuxfj.sHtML

Py:   max(arr);  min(arr)
来源：http://wap.zdbjq.cn/Article/details/ggoqrkima.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gwtfgknhl.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://blog.hesvh.cn/Article/details/guqxgcaac.sHtML

TS:   Math.max(...arr);
来源：http://www.share.zdbjq.cn/Article/details/gpmnazmma.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://read.share.hesvh.cn/Article/details/gsrpwjisq.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://3g.hesvh.cn/Article/details/gihgcwzdv.sHtML

Ruby: arr.max;  arr.min
来源：http://baike.hesvh.cn/Article/details/gdtrsffou.sHtML

C#:   list.Max();  list.Min()
来源：http://www.share.fehbvm.com/Article/details/giyljhcaz.sHtML

[D18] 扁平化嵌套数组
来源：http://read.share.fehbvm.com/Article/details/gcnzceeec.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wap.zdbjq.cn/Article/details/grubahdvk.sHtML

PHP:  array_merge(...$nested);
来源：http://blog.hesvh.cn/Article/details/gjawkbefm.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://3g.zdbjq.cn/Article/details/gnwmamskr.sHtML

TS:   nested.flat();
来源：http://read.share.hesvh.cn/Article/details/gnlzltjex.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.blog.hesvh.cn/Article/details/gfmyimorh.sHtML

Go:   // 手写双层循环
来源：http://read.share.hesvh.cn/Article/details/gxqlprhcy.sHtML

Ruby: nested.flatten
来源：http://m.share.hesvh.cn/Article/details/gfscgezti.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.blog.fehbvm.com/Article/details/gixgjnake.sHtML

[D19] 按字段分组
来源：http://blog.zdbjq.cn/Article/details/gcugcqlot.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wap.hesvh.cn/Article/details/gzsbguweb.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://blog.hesvh.cn/Article/details/ghfrvpysk.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://blog.fehbvm.com/Article/details/gsyiyaayv.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://m.share.fehbvm.com/Article/details/gethziwls.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://baike.zdbjq.cn/Article/details/gayezezot.sHtML

Go:   // 手写 map[string][]T
来源：http://www.blog.zdbjq.cn/Article/details/gfusryxsu.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://blog.hesvh.cn/Article/details/gtibsefom.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://3g.hesvh.cn/Article/details/gxixquudt.sHtML

[D20] 统计每个元素出现次数
来源：http://www.share.zdbjq.cn/Article/details/gatauocnh.sHtML

Py:   Counter(arr)
来源：http://3g.hesvh.cn/Article/details/goqkvgxqe.sHtML

PHP:  array_count_values($arr);
来源：http://blog.zdbjq.cn/Article/details/geescgrae.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.fehbvm.com/Article/details/glslkmbfx.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.hesvh.cn/Article/details/gryykjmpi.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.blog.fehbvm.com/Article/details/gaagetjnr.sHtML

Go:   // 手写 map[T]int
来源：http://3g.fehbvm.com/Article/details/gvexddiwf.sHtML

Ruby: arr.tally
来源：http://m.share.hesvh.cn/Article/details/gxgtrexzl.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://3g.fehbvm.com/Article/details/gfafsqoyb.sHtML

[D21] 判断是否包含某元素
来源：http://blog.zdbjq.cn/Article/details/gycycrzzn.sHtML

Py:   x in arr
来源：http://www.m.share.fehbvm.com/Article/details/ghavmbajd.sHtML

PHP:  in_array($x, $arr, true);
来源：http://wap.fehbvm.com/Article/details/gsdiaplgs.sHtML

JS:   arr.includes(x)
来源：http://3g.zdbjq.cn/Article/details/glsbqvrxc.sHtML

TS:   arr.includes(x)
来源：http://www.share.hesvh.cn/Article/details/ghzlsmebq.sHtML

Java: list.contains(x)
来源：http://blog.fehbvm.com/Article/details/gncrdsqxl.sHtML

Go:   slices.Contains(arr, x)
来源：http://mobile.zdbjq.cn/Article/details/gwigrlbdz.sHtML

Ruby: arr.include?(x)
来源：http://read.share.fehbvm.com/Article/details/ghrqaprrd.sHtML

C#:   list.Contains(x)
来源：http://www.share.fehbvm.com/Article/details/gipoznapq.sHtML

[D22] 复制数组（避免共享引用）
来源：http://wap.zdbjq.cn/Article/details/gflvfqtog.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://baike.zdbjq.cn/Article/details/gmcynftfw.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.m.share.fehbvm.com/Article/details/gevssvxmu.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://blog.hesvh.cn/Article/details/gfkjrqnzx.sHtML

TS:   [...arr];
来源：http://wap.fehbvm.com/Article/details/gbpxnrrgt.sHtML

Java: new ArrayList<>(list);
来源：http://www.m.share.hesvh.cn/Article/details/gpzgrdeby.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.m.share.hesvh.cn/Article/details/gpyjoizsi.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.share.zdbjq.cn/Article/details/gbooenqtc.sHtML

C#:   new List<int>(list);
来源：http://read.share.zdbjq.cn/Article/details/gapqssgwx.sHtML

[D23] reduce 累积计算
来源：http://www.share.fehbvm.com/Article/details/glykunlyc.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://blog.fehbvm.com/Article/details/gwtnajrts.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.share.hesvh.cn/Article/details/gddtsbaxr.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.fehbvm.com/Article/details/gisxxfwiv.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.zdbjq.cn/Article/details/gvnxrwjsv.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://3g.hesvh.cn/Article/details/gekmmggwd.sHtML

Go:   // 手写循环
来源：http://3g.fehbvm.com/Article/details/gwiqhvumb.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://read.share.fehbvm.com/Article/details/glifgtzxu.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mobile.fehbvm.com/Article/details/gyyypwmyz.sHtML

[D24] 字典 / Map 基本操作
来源：http://3g.zdbjq.cn/Article/details/gzxhgjtpo.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.blog.fehbvm.com/Article/details/gkxexigwy.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://baike.hesvh.cn/Article/details/gldnkekhh.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wap.hesvh.cn/Article/details/gcnpiampl.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://m.share.zdbjq.cn/Article/details/glcdalifm.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://baike.fehbvm.com/Article/details/grlqwvmdq.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://m.share.zdbjq.cn/Article/details/gygtoewsu.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://m.share.zdbjq.cn/Article/details/guwijgoqp.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://read.share.fehbvm.com/Article/details/gkchipybp.sHtML

[D25] Set 集合去重与交并差
来源：http://www.blog.zdbjq.cn/Article/details/gllkybbxa.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.share.hesvh.cn/Article/details/gdsnoohhl.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mobile.fehbvm.com/Article/details/gctrsjzwt.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.m.share.hesvh.cn/Article/details/gifmhvtqr.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.blog.fehbvm.com/Article/details/ggcuripmf.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.m.share.zdbjq.cn/Article/details/geeotyjdi.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://blog.zdbjq.cn/Article/details/gvmazxeef.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mobile.zdbjq.cn/Article/details/gwdzbfzhw.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://baike.zdbjq.cn/Article/details/galiotuif.sHtML

[D26] 数组转字符串
来源：http://wap.zdbjq.cn/Article/details/gmckmufwx.sHtML

Py:   ", ".join(map(str, arr))
来源：http://baike.zdbjq.cn/Article/details/gejekcdng.sHtML

PHP:  implode(", ", $arr);
来源：http://wap.zdbjq.cn/Article/details/gujkffgqc.sHtML

JS:   arr.join(", ")
来源：http://www.m.share.hesvh.cn/Article/details/gdqqjxvcx.sHtML

TS:   arr.join(", ")
来源：http://baike.zdbjq.cn/Article/details/gedbkjbcs.sHtML

Java: String.join(", ", list)
来源：http://3g.fehbvm.com/Article/details/gxekiznua.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.blog.fehbvm.com/Article/details/gcklgxkgu.sHtML

Ruby: arr.join(", ")
来源：http://www.share.zdbjq.cn/Article/details/gigvozvpv.sHtML

C#:   string.Join(", ", list)
来源：http://wap.fehbvm.com/Article/details/gpuqanurw.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gkuznoyqy.sHtML

E. 字符串处理
来源：http://www.share.zdbjq.cn/Article/details/goufqtoer.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gpmoxenou.sHtML

[E01] 拼接字符串
来源：http://m.share.zdbjq.cn/Article/details/gsrojkkqy.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.m.share.hesvh.cn/Article/details/gnejjtcmp.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.m.share.fehbvm.com/Article/details/gkmqrenhn.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.zdbjq.cn/Article/details/gflzorkoz.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.hesvh.cn/Article/details/ggwzrfmcc.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://mobile.fehbvm.com/Article/details/gzgrhjoky.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://mobile.fehbvm.com/Article/details/gtdjpzpve.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mobile.hesvh.cn/Article/details/gvmtcgupa.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.share.zdbjq.cn/Article/details/ghuhtyfil.sHtML

[E02] 重复字符串
来源：http://www.m.share.hesvh.cn/Article/details/gscyyzcfc.sHtML

Py:   "ab" * 3
来源：http://mobile.fehbvm.com/Article/details/glyxyjmmt.sHtML

PHP:  str_repeat("ab", 3);
来源：http://3g.fehbvm.com/Article/details/ghabimujo.sHtML

JS:   "ab".repeat(3)
来源：http://www.share.zdbjq.cn/Article/details/gfpatjtmt.sHtML

TS:   "ab".repeat(3)
来源：http://baike.fehbvm.com/Article/details/gxfvnzbxg.sHtML

Java: "ab".repeat(3)
来源：http://read.share.zdbjq.cn/Article/details/gcfowmhop.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.blog.zdbjq.cn/Article/details/ghkovrbpl.sHtML

Ruby: "ab" * 3
来源：http://baike.hesvh.cn/Article/details/gklbszlte.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://3g.zdbjq.cn/Article/details/gesgbrttv.sHtML

[E03] 截取子串
来源：http://3g.zdbjq.cn/Article/details/gkcospdlp.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.blog.fehbvm.com/Article/details/gynqrbzsn.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://baike.fehbvm.com/Article/details/glrqsqgew.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.share.zdbjq.cn/Article/details/gdvqjopdh.sHtML

TS:   s.slice(1, 4)
来源：http://3g.fehbvm.com/Article/details/gedeaokuw.sHtML

Java: s.substring(1, 4)
来源：http://www.m.share.fehbvm.com/Article/details/giayanqlb.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://mobile.fehbvm.com/Article/details/gqdajgqyu.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://mobile.zdbjq.cn/Article/details/guriifdgs.sHtML

C#:   s.Substring(1, 3)
来源：http://mobile.fehbvm.com/Article/details/gnpeupcdr.sHtML

[E04] 查找子串位置
来源：http://3g.fehbvm.com/Article/details/gobeathqz.sHtML

Py:   s.find("x");  s.index("x")
来源：http://m.share.hesvh.cn/Article/details/gzzkxxwxw.sHtML

PHP:  strpos($s, "x");
来源：http://www.blog.fehbvm.com/Article/details/gfpmeydgo.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://blog.fehbvm.com/Article/details/gcldzwymv.sHtML

TS:   s.indexOf("x")
来源：http://3g.fehbvm.com/Article/details/ggdzxbedi.sHtML

Java: s.indexOf("x")
来源：http://mobile.fehbvm.com/Article/details/gdhxhaypo.sHtML

Go:   strings.Index(s, "x")
来源：http://www.share.hesvh.cn/Article/details/gioisfptc.sHtML

Ruby: s.index("x")
来源：http://3g.zdbjq.cn/Article/details/gznpfaefr.sHtML

C#:   s.IndexOf("x")
来源：http://www.m.share.fehbvm.com/Article/details/gamdnflcq.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://baike.zdbjq.cn/Article/details/gwkdtlhmu.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.m.share.zdbjq.cn/Article/details/gfppacstk.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wap.hesvh.cn/Article/details/gbcsrqwss.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.zdbjq.cn/Article/details/gckhrunhp.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.blog.fehbvm.com/Article/details/gavjdotvs.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.hesvh.cn/Article/details/gakrgpqfy.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://3g.zdbjq.cn/Article/details/gvzbkcxna.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://m.share.hesvh.cn/Article/details/gwnznscbn.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.blog.zdbjq.cn/Article/details/ggnewxukl.sHtML

[E06] 替换子串
来源：http://blog.fehbvm.com/Article/details/gztrzdqjw.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://wap.zdbjq.cn/Article/details/gyszzpsag.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.blog.fehbvm.com/Article/details/grtgttpuk.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.zdbjq.cn/Article/details/glmrfioze.sHtML

TS:   s.replaceAll("a", "b")
来源：http://mobile.zdbjq.cn/Article/details/gbfjcwycd.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.fehbvm.com/Article/details/gsjxqarqg.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.m.share.zdbjq.cn/Article/details/gylqpbhng.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://baike.hesvh.cn/Article/details/gpklcbrqw.sHtML

C#:   s.Replace("a", "b")
来源：http://m.share.fehbvm.com/Article/details/gffzjrftf.sHtML

[E07] 按分隔符拆分
来源：http://www.share.fehbvm.com/Article/details/gccjcvdqo.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.share.fehbvm.com/Article/details/gxcjclxgc.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://wap.fehbvm.com/Article/details/glggrlksu.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://3g.zdbjq.cn/Article/details/guwcmmwop.sHtML

TS:   s.split(",")
来源：http://m.share.zdbjq.cn/Article/details/gdzgbnvxl.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://read.share.fehbvm.com/Article/details/gcodvyvqf.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://mobile.zdbjq.cn/Article/details/gosyrfobl.sHtML

Ruby: s.split(",");  s.split
来源：http://3g.zdbjq.cn/Article/details/gmeaavble.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://read.share.hesvh.cn/Article/details/gmwvwcvjr.sHtML

[E08] 数组按分隔符合并
来源：http://www.share.fehbvm.com/Article/details/giqotmihe.sHtML

Py:   ",".join(items)
来源：http://wap.fehbvm.com/Article/details/gsnhxqnfi.sHtML

PHP:  implode(",", $items);
来源：http://3g.fehbvm.com/Article/details/gcduqpizw.sHtML

JS:   items.join(",")
来源：http://baike.hesvh.cn/Article/details/gvzmhgmvr.sHtML

TS:   items.join(",")
来源：http://m.share.zdbjq.cn/Article/details/gmcthapjm.sHtML

Java: String.join(",", items)
来源：http://baike.fehbvm.com/Article/details/gxmqeensc.sHtML

Go:   strings.Join(items, ",")
来源：http://m.share.fehbvm.com/Article/details/gsjhpznai.sHtML

Ruby: items.join(",")
来源：http://baike.hesvh.cn/Article/details/gilydxjrr.sHtML

C#:   string.Join(",", items)
来源：http://wap.hesvh.cn/Article/details/ghbardjed.sHtML

[E09] 去除所有空白字符
来源：http://www.blog.fehbvm.com/Article/details/gblumsdrs.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://3g.zdbjq.cn/Article/details/grcoszkbp.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wap.fehbvm.com/Article/details/grmeyceig.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://read.share.fehbvm.com/Article/details/gspefsywq.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://mobile.fehbvm.com/Article/details/gtjvyckqd.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://baike.fehbvm.com/Article/details/ghxdrszes.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://3g.hesvh.cn/Article/details/gldsqbaml.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.m.share.zdbjq.cn/Article/details/gizbilfix.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://baike.zdbjq.cn/Article/details/gjbcnuoda.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.m.share.fehbvm.com/Article/details/gwdfqsykz.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://read.share.fehbvm.com/Article/details/gprpxzwni.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://3g.hesvh.cn/Article/details/ghtxhrptd.sHtML

JS:   "7".padStart(3, "0")
来源：http://wap.hesvh.cn/Article/details/gfdshltbz.sHtML

TS:   "7".padStart(3, "0")
来源：http://3g.zdbjq.cn/Article/details/gzllwcdxa.sHtML

Java: String.format("%03d", 7)
来源：http://wap.zdbjq.cn/Article/details/gtkksgeim.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://3g.hesvh.cn/Article/details/gsuqlsavt.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://blog.zdbjq.cn/Article/details/gtolqaecl.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://mobile.hesvh.cn/Article/details/gihvonygx.sHtML

[E11] 反转字符串
来源：http://www.share.zdbjq.cn/Article/details/gspcjbzrt.sHtML

Py:   s[::-1]
来源：http://3g.hesvh.cn/Article/details/gusdwatxp.sHtML

PHP:  strrev($s);
来源：http://m.share.fehbvm.com/Article/details/gmlghlsbs.sHtML

JS:   [...s].reverse().join("")
来源：http://mobile.zdbjq.cn/Article/details/ggyardmjc.sHtML

TS:   [...s].reverse().join("")
来源：http://blog.zdbjq.cn/Article/details/gygbpmrdj.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://baike.hesvh.cn/Article/details/glraetyzx.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://wap.zdbjq.cn/Article/details/gofwtffqa.sHtML

Ruby: s.reverse
来源：http://www.m.share.fehbvm.com/Article/details/gpurwxzcm.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://blog.hesvh.cn/Article/details/gkfzzwwsr.sHtML

[E12] 统计某字符出现次数
来源：http://mobile.fehbvm.com/Article/details/gdjjosiax.sHtML

Py:   s.count("a")
来源：http://3g.fehbvm.com/Article/details/gjfmsqfwg.sHtML

PHP:  substr_count($s, "a");
来源：http://www.share.fehbvm.com/Article/details/gfsyzywvp.sHtML

JS:   s.split("a").length - 1
来源：http://m.share.fehbvm.com/Article/details/grpjoebrf.sHtML

TS:   s.split("a").length - 1
来源：http://blog.zdbjq.cn/Article/details/gtebvyrts.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://3g.hesvh.cn/Article/details/gtjxpykzx.sHtML


<!-- 参考信息 -->