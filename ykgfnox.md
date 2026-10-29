代发 wailian999

Go:   arr[0]; arr[0] = 9
来源：http://baike.hesvh.cn/Article/details/gxgwzgmbv.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.fehbvm.com/Article/details/gvafjxqih.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mobile.hesvh.cn/Article/details/gwwhjazuo.sHtML

[D06] 数组长度
来源：http://www.share.zdbjq.cn/Article/details/giapyakmk.sHtML

Py:   len(arr)
来源：http://baike.zdbjq.cn/Article/details/gpwswvkbr.sHtML

PHP:  count($arr);
来源：http://www.blog.zdbjq.cn/Article/details/gyacjyxjs.sHtML

JS:   arr.length
来源：http://baike.hesvh.cn/Article/details/gaomcuyrt.sHtML

TS:   arr.length
来源：http://baike.fehbvm.com/Article/details/gjzmomijp.sHtML

Java: list.size();
来源：http://read.share.hesvh.cn/Article/details/gquklywve.sHtML

Go:   len(arr)
来源：http://wap.zdbjq.cn/Article/details/ggvkcctii.sHtML

Ruby: arr.length; arr.size
来源：http://read.share.fehbvm.com/Article/details/gsgxrifcm.sHtML

C#:   list.Count;
来源：http://3g.fehbvm.com/Article/details/gvcrxmaqa.sHtML

[D07] 切片 / 取子数组
来源：http://3g.zdbjq.cn/Article/details/gzeufizrw.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://baike.fehbvm.com/Article/details/gsqcmlytl.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://3g.fehbvm.com/Article/details/gtevzkybo.sHtML

JS:   arr.slice(1, 4);
来源：http://www.m.share.hesvh.cn/Article/details/ggeyukwfe.sHtML

TS:   arr.slice(1, 4);
来源：http://baike.hesvh.cn/Article/details/gpuqthznd.sHtML

Java: list.subList(1, 4);
来源：http://wap.hesvh.cn/Article/details/gmwguynma.sHtML

Go:   arr[1:4]
来源：http://baike.fehbvm.com/Article/details/gqabvrbqj.sHtML

Ruby: arr[1, 3]
来源：http://baike.zdbjq.cn/Article/details/glpbraqxg.sHtML

C#:   list.GetRange(1, 3);
来源：http://baike.fehbvm.com/Article/details/gakszrgzr.sHtML

[D08] 合并两个数组
来源：http://wap.fehbvm.com/Article/details/gifmzpekz.sHtML

Py:   a + b;  a.extend(b)
来源：http://baike.zdbjq.cn/Article/details/gsuvbzxtr.sHtML

PHP:  array_merge($a, $b);
来源：http://mobile.hesvh.cn/Article/details/gpjeoxqex.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.share.zdbjq.cn/Article/details/gvhhtvhzj.sHtML

TS:   [...a, ...b];
来源：http://mobile.fehbvm.com/Article/details/gpxxjtiav.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://m.share.hesvh.cn/Article/details/gdpmyajmu.sHtML

Go:   append(a, b...)
来源：http://m.share.zdbjq.cn/Article/details/gxbarintz.sHtML

Ruby: a + b;  a.concat(b)
来源：http://3g.zdbjq.cn/Article/details/guvmwdpfk.sHtML

C#:   a.Concat(b).ToList()
来源：http://baike.hesvh.cn/Article/details/gnujraabe.sHtML

[D09] 排序（升序）
来源：http://wap.hesvh.cn/Article/details/gnilljlzj.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.fehbvm.com/Article/details/gzgcvlfae.sHtML

PHP:  sort($arr);
来源：http://blog.hesvh.cn/Article/details/gbivkoakv.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://baike.fehbvm.com/Article/details/gmcsyklrd.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://m.share.zdbjq.cn/Article/details/gbpnxrgdq.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://baike.hesvh.cn/Article/details/gkdcctmov.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://read.share.zdbjq.cn/Article/details/gebdorsqy.sHtML

Ruby: arr.sort
来源：http://mobile.zdbjq.cn/Article/details/gpzvbirxe.sHtML

C#:   list.Sort();
来源：http://www.share.hesvh.cn/Article/details/gjdvcmiuq.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://blog.fehbvm.com/Article/details/gamalemsu.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://blog.hesvh.cn/Article/details/gdblwurri.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.zdbjq.cn/Article/details/gfchstldf.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.fehbvm.com/Article/details/gmujsbzsm.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.hesvh.cn/Article/details/gwvibddwr.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://blog.hesvh.cn/Article/details/gmqvmbrmt.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://mobile.zdbjq.cn/Article/details/glxhsylzo.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://read.share.fehbvm.com/Article/details/grdmxfpwh.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://read.share.fehbvm.com/Article/details/gzcapnqwz.sHtML

[D11] 反转数组
来源：http://read.share.fehbvm.com/Article/details/gkqblwbyv.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://read.share.hesvh.cn/Article/details/godkxomap.sHtML

PHP:  array_reverse($arr);
来源：http://m.share.zdbjq.cn/Article/details/georsvkru.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://3g.fehbvm.com/Article/details/gwyuczekh.sHtML

TS:   [...arr].reverse();
来源：http://mobile.fehbvm.com/Article/details/grwptyhkc.sHtML

Java: Collections.reverse(list);
来源：http://mobile.zdbjq.cn/Article/details/guhsrjnwf.sHtML

Go:   slices.Reverse(arr)
来源：http://mobile.zdbjq.cn/Article/details/gnbyyipry.sHtML

Ruby: arr.reverse
来源：http://baike.zdbjq.cn/Article/details/gcihrvueq.sHtML

C#:   list.Reverse();
来源：http://mobile.fehbvm.com/Article/details/gjbjguzco.sHtML

[D12] 查找元素下标
来源：http://www.blog.fehbvm.com/Article/details/grgasvsqd.sHtML

Py:   arr.index(x);  x in arr
来源：http://blog.zdbjq.cn/Article/details/gmatiinea.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://wap.fehbvm.com/Article/details/gcfxawirt.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.hesvh.cn/Article/details/ggkxwafbr.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.fehbvm.com/Article/details/gyoxgjfqa.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.share.hesvh.cn/Article/details/gfmnamsvk.sHtML

Go:   slices.Index(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/gcmkghckl.sHtML

Ruby: arr.index(x)
来源：http://m.share.hesvh.cn/Article/details/guuvoghyc.sHtML

C#:   list.IndexOf(x);
来源：http://wap.fehbvm.com/Article/details/gqysoigwf.sHtML

[D13] 过滤（保留满足条件的）
来源：http://3g.fehbvm.com/Article/details/gtfutazya.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://mobile.fehbvm.com/Article/details/gkkxihgha.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gjiupxfrl.sHtML

JS:   arr.filter(x => x > 3)
来源：http://m.share.fehbvm.com/Article/details/gdggdhmaq.sHtML

TS:   arr.filter(x => x > 3)
来源：http://blog.fehbvm.com/Article/details/gyxfdunxx.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://3g.fehbvm.com/Article/details/gnbhybxgj.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mobile.zdbjq.cn/Article/details/gopqiehbm.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://m.share.fehbvm.com/Article/details/gnhmvgzqb.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://blog.hesvh.cn/Article/details/gxuvvxexj.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.share.hesvh.cn/Article/details/gkcgwpcic.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://blog.fehbvm.com/Article/details/gerlcqfnu.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.share.zdbjq.cn/Article/details/ghoxwojin.sHtML

JS:   arr.map(x => x * 2)
来源：http://read.share.zdbjq.cn/Article/details/gllzpxsgb.sHtML

TS:   arr.map(x => x * 2)
来源：http://baike.fehbvm.com/Article/details/gywuwnrtr.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.share.zdbjq.cn/Article/details/gloufgtnk.sHtML

Go:   // 手写循环
来源：http://mobile.hesvh.cn/Article/details/glkcolbej.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.m.share.hesvh.cn/Article/details/gwsaniogl.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://wap.fehbvm.com/Article/details/gtoaqhopy.sHtML

[D15] 去重
来源：http://www.share.fehbvm.com/Article/details/gxwwaoihd.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://m.share.hesvh.cn/Article/details/goohfvhfo.sHtML

PHP:  array_unique($arr);
来源：http://www.blog.fehbvm.com/Article/details/grpzolbby.sHtML

JS:   [...new Set(arr)]
来源：http://read.share.hesvh.cn/Article/details/gukucpxkc.sHtML

TS:   [...new Set(arr)]
来源：http://www.m.share.zdbjq.cn/Article/details/gvrfvzlsy.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://read.share.fehbvm.com/Article/details/gwwmvsrdz.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://mobile.hesvh.cn/Article/details/ginyqtohn.sHtML

Ruby: arr.uniq
来源：http://www.m.share.hesvh.cn/Article/details/gmxyknhjt.sHtML

C#:   list.Distinct().ToList()
来源：http://blog.zdbjq.cn/Article/details/gexmtlzud.sHtML

[D16] 求和与平均值
来源：http://mobile.fehbvm.com/Article/details/glwikuzds.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://mobile.zdbjq.cn/Article/details/gbjjvyfoa.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://3g.fehbvm.com/Article/details/grbdscckh.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.zdbjq.cn/Article/details/gcgfmoilb.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.zdbjq.cn/Article/details/gkplsgjji.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://m.share.zdbjq.cn/Article/details/gjeuxhipa.sHtML

Go:   // 手写循环累加
来源：http://blog.zdbjq.cn/Article/details/girometwt.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://baike.fehbvm.com/Article/details/gvttanynu.sHtML

C#:   list.Sum();  list.Average()
来源：http://baike.fehbvm.com/Article/details/gfysfifle.sHtML

[D17] 最大值与最小值
来源：http://mobile.fehbvm.com/Article/details/geeckxxcj.sHtML

Py:   max(arr);  min(arr)
来源：http://read.share.fehbvm.com/Article/details/gzfdnjlyx.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.blog.hesvh.cn/Article/details/grzcaovny.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://3g.hesvh.cn/Article/details/gxoqzclpz.sHtML

TS:   Math.max(...arr);
来源：http://read.share.hesvh.cn/Article/details/gtsprcigq.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://mobile.hesvh.cn/Article/details/gyyteipvg.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wap.zdbjq.cn/Article/details/gacruvkqx.sHtML

Ruby: arr.max;  arr.min
来源：http://mobile.zdbjq.cn/Article/details/gylfmfaer.sHtML

C#:   list.Max();  list.Min()
来源：http://www.m.share.zdbjq.cn/Article/details/gryljmmpv.sHtML

[D18] 扁平化嵌套数组
来源：http://read.share.hesvh.cn/Article/details/ggehgppxx.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://m.share.fehbvm.com/Article/details/gozyucvhs.sHtML

PHP:  array_merge(...$nested);
来源：http://blog.hesvh.cn/Article/details/gjlpynzwp.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wap.zdbjq.cn/Article/details/gbrppdexb.sHtML

TS:   nested.flat();
来源：http://m.share.hesvh.cn/Article/details/gcfsvaqsf.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.blog.hesvh.cn/Article/details/gwscarqim.sHtML

Go:   // 手写双层循环
来源：http://www.blog.fehbvm.com/Article/details/gaqrfgwkz.sHtML

Ruby: nested.flatten
来源：http://blog.fehbvm.com/Article/details/gdriwxyqg.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://mobile.fehbvm.com/Article/details/gwckdgzil.sHtML

[D19] 按字段分组
来源：http://www.m.share.fehbvm.com/Article/details/gxfayxyde.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://3g.zdbjq.cn/Article/details/gymrllkzr.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://read.share.fehbvm.com/Article/details/gcjmivegv.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.blog.zdbjq.cn/Article/details/glaqoycpj.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://read.share.zdbjq.cn/Article/details/gntbrfdxm.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://baike.hesvh.cn/Article/details/gwisvzeie.sHtML

Go:   // 手写 map[string][]T
来源：http://www.share.hesvh.cn/Article/details/gokadfxpb.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://3g.hesvh.cn/Article/details/gpaeqlhtl.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wap.hesvh.cn/Article/details/gtkvtjjid.sHtML

[D20] 统计每个元素出现次数
来源：http://www.blog.hesvh.cn/Article/details/ggztyeaev.sHtML

Py:   Counter(arr)
来源：http://www.share.zdbjq.cn/Article/details/gbsnnxzck.sHtML

PHP:  array_count_values($arr);
来源：http://blog.hesvh.cn/Article/details/gzgrwocrm.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.zdbjq.cn/Article/details/geoecwhnp.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.fehbvm.com/Article/details/gctpemzxq.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://3g.hesvh.cn/Article/details/gpawnhrlx.sHtML

Go:   // 手写 map[T]int
来源：http://3g.zdbjq.cn/Article/details/gpakmdjic.sHtML

Ruby: arr.tally
来源：http://m.share.fehbvm.com/Article/details/gprkubiqy.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wap.hesvh.cn/Article/details/gclklpntb.sHtML

[D21] 判断是否包含某元素
来源：http://www.share.zdbjq.cn/Article/details/goglkledg.sHtML

Py:   x in arr
来源：http://www.share.fehbvm.com/Article/details/gpqxfamgm.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.share.zdbjq.cn/Article/details/gyqperxiw.sHtML

JS:   arr.includes(x)
来源：http://www.share.hesvh.cn/Article/details/gcjcsjtqm.sHtML

TS:   arr.includes(x)
来源：http://www.blog.zdbjq.cn/Article/details/gtelmlpzh.sHtML

Java: list.contains(x)
来源：http://3g.zdbjq.cn/Article/details/gkryjkfqk.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.blog.fehbvm.com/Article/details/gxscqcflf.sHtML

Ruby: arr.include?(x)
来源：http://m.share.hesvh.cn/Article/details/gqscvifuh.sHtML

C#:   list.Contains(x)
来源：http://mobile.zdbjq.cn/Article/details/godkxfarh.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.blog.hesvh.cn/Article/details/ggjaoywlm.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.blog.hesvh.cn/Article/details/gzrltrujy.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://m.share.zdbjq.cn/Article/details/gqgkytppi.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gxadxujig.sHtML

TS:   [...arr];
来源：http://wap.zdbjq.cn/Article/details/gzyczxxxn.sHtML

Java: new ArrayList<>(list);
来源：http://www.share.fehbvm.com/Article/details/gfzekbupc.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.blog.zdbjq.cn/Article/details/gddgdrwtz.sHtML

Ruby: arr.dup;  arr.clone
来源：http://3g.hesvh.cn/Article/details/gvakphgwq.sHtML

C#:   new List<int>(list);
来源：http://wap.fehbvm.com/Article/details/gdkulxbbp.sHtML

[D23] reduce 累积计算
来源：http://baike.fehbvm.com/Article/details/gxadsjbst.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://mobile.zdbjq.cn/Article/details/goffiujgc.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.share.fehbvm.com/Article/details/gbjhvknzk.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.fehbvm.com/Article/details/gbosaszve.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.fehbvm.com/Article/details/gbwpqbjpa.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://3g.hesvh.cn/Article/details/ghfxoyfzr.sHtML

Go:   // 手写循环
来源：http://blog.zdbjq.cn/Article/details/giszzytuo.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.m.share.hesvh.cn/Article/details/gmffmiaje.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.blog.hesvh.cn/Article/details/gupzoqewo.sHtML

[D24] 字典 / Map 基本操作
来源：http://blog.zdbjq.cn/Article/details/gpescmvnc.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://baike.zdbjq.cn/Article/details/gqnaozynt.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://wap.fehbvm.com/Article/details/grixenffq.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.blog.fehbvm.com/Article/details/gzzsedwxg.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://baike.hesvh.cn/Article/details/gsdryijrc.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://read.share.zdbjq.cn/Article/details/gkcecyqsu.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://read.share.zdbjq.cn/Article/details/glcvmlnyi.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.m.share.hesvh.cn/Article/details/gjamxbbwk.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://read.share.hesvh.cn/Article/details/gdxpppvta.sHtML

[D25] Set 集合去重与交并差
来源：http://blog.zdbjq.cn/Article/details/gwylrkaui.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://3g.hesvh.cn/Article/details/gqxyjqdau.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wap.zdbjq.cn/Article/details/gbccaqjia.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://3g.hesvh.cn/Article/details/ggolnclda.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://baike.zdbjq.cn/Article/details/gtybhyzwi.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.share.zdbjq.cn/Article/details/gqqkvswxa.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.share.zdbjq.cn/Article/details/gmlkrfwkh.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.share.hesvh.cn/Article/details/gzumqtemp.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://blog.hesvh.cn/Article/details/ghruelpqz.sHtML

[D26] 数组转字符串
来源：http://www.m.share.hesvh.cn/Article/details/ggyhscmhw.sHtML

Py:   ", ".join(map(str, arr))
来源：http://baike.hesvh.cn/Article/details/gbadeocel.sHtML

PHP:  implode(", ", $arr);
来源：http://www.m.share.fehbvm.com/Article/details/gsiyhiioc.sHtML

JS:   arr.join(", ")
来源：http://blog.zdbjq.cn/Article/details/goophrsfu.sHtML

TS:   arr.join(", ")
来源：http://m.share.zdbjq.cn/Article/details/gzltohqee.sHtML

Java: String.join(", ", list)
来源：http://www.blog.zdbjq.cn/Article/details/gdgdhbtez.sHtML

Go:   strings.Join(strs, ", ")
来源：http://read.share.fehbvm.com/Article/details/gbxnqkjnw.sHtML

Ruby: arr.join(", ")
来源：http://m.share.hesvh.cn/Article/details/gzugihljm.sHtML

C#:   string.Join(", ", list)
来源：http://m.share.fehbvm.com/Article/details/ggfdlgbav.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gpqtrhdpz.sHtML

E. 字符串处理
来源：http://www.m.share.fehbvm.com/Article/details/goelfxckc.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gfyztimqj.sHtML

[E01] 拼接字符串
来源：http://blog.hesvh.cn/Article/details/glevfnjfx.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://3g.zdbjq.cn/Article/details/gkhigvrql.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://read.share.fehbvm.com/Article/details/gjplyycnt.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.hesvh.cn/Article/details/ghwhgwvrz.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.fehbvm.com/Article/details/gurypggap.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://3g.zdbjq.cn/Article/details/ghzdnulnc.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.blog.zdbjq.cn/Article/details/gioqjesgk.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.share.fehbvm.com/Article/details/giuffiaub.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.m.share.hesvh.cn/Article/details/gdbtiihgj.sHtML

[E02] 重复字符串
来源：http://www.m.share.hesvh.cn/Article/details/gtibdlvkz.sHtML

Py:   "ab" * 3
来源：http://baike.fehbvm.com/Article/details/gfqyoecuh.sHtML

PHP:  str_repeat("ab", 3);
来源：http://blog.zdbjq.cn/Article/details/gacfvrzyd.sHtML

JS:   "ab".repeat(3)
来源：http://blog.zdbjq.cn/Article/details/gosgmzmff.sHtML

TS:   "ab".repeat(3)
来源：http://baike.zdbjq.cn/Article/details/gqbqjdsms.sHtML

Java: "ab".repeat(3)
来源：http://www.blog.fehbvm.com/Article/details/gssovbzwo.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.m.share.hesvh.cn/Article/details/gspwfrnmq.sHtML

Ruby: "ab" * 3
来源：http://wap.hesvh.cn/Article/details/gvvumfhwe.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.share.fehbvm.com/Article/details/gefdmpugv.sHtML

[E03] 截取子串
来源：http://wap.hesvh.cn/Article/details/gudgyxdvm.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://3g.zdbjq.cn/Article/details/geohecsxm.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.blog.fehbvm.com/Article/details/gwissxpfi.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://blog.zdbjq.cn/Article/details/gdzxupvxk.sHtML

TS:   s.slice(1, 4)
来源：http://read.share.zdbjq.cn/Article/details/gipasfvzu.sHtML

Java: s.substring(1, 4)
来源：http://baike.fehbvm.com/Article/details/gtwcsuupo.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://blog.fehbvm.com/Article/details/gclzhgulz.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://m.share.fehbvm.com/Article/details/gpqwbjgwi.sHtML

C#:   s.Substring(1, 3)
来源：http://www.blog.hesvh.cn/Article/details/gzkoksylp.sHtML

[E04] 查找子串位置
来源：http://blog.fehbvm.com/Article/details/gaznlsgno.sHtML

Py:   s.find("x");  s.index("x")
来源：http://mobile.fehbvm.com/Article/details/gamykmrsl.sHtML

PHP:  strpos($s, "x");
来源：http://baike.hesvh.cn/Article/details/gixwuqlah.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://mobile.fehbvm.com/Article/details/gzpqgsvaz.sHtML

TS:   s.indexOf("x")
来源：http://wap.hesvh.cn/Article/details/gbxfcfjaw.sHtML

Java: s.indexOf("x")
来源：http://wap.fehbvm.com/Article/details/grlpjriyf.sHtML

Go:   strings.Index(s, "x")
来源：http://m.share.hesvh.cn/Article/details/gqwrkyfnw.sHtML

Ruby: s.index("x")
来源：http://www.blog.zdbjq.cn/Article/details/gyalkqqth.sHtML

C#:   s.IndexOf("x")
来源：http://www.m.share.hesvh.cn/Article/details/ggplrptoz.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.share.hesvh.cn/Article/details/gazgrqjqb.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://m.share.hesvh.cn/Article/details/gzpxwkssu.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://baike.hesvh.cn/Article/details/gpkjudrvj.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.fehbvm.com/Article/details/gvwnuiiws.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.m.share.hesvh.cn/Article/details/gchbholxf.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.fehbvm.com/Article/details/gdcguiizw.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://read.share.zdbjq.cn/Article/details/gjketrjrn.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://mobile.hesvh.cn/Article/details/gjoexwvvc.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://blog.zdbjq.cn/Article/details/glodarpdq.sHtML

[E06] 替换子串
来源：http://baike.hesvh.cn/Article/details/gljlmvnyu.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://blog.fehbvm.com/Article/details/gjdkpyhpx.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://blog.hesvh.cn/Article/details/gzjrbdcxv.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/grgoygkjf.sHtML

TS:   s.replaceAll("a", "b")
来源：http://baike.hesvh.cn/Article/details/gwrydxyhd.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.hesvh.cn/Article/details/gplsllfxe.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://read.share.fehbvm.com/Article/details/gnqaaefye.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://3g.hesvh.cn/Article/details/gtavsmeur.sHtML

C#:   s.Replace("a", "b")
来源：http://read.share.fehbvm.com/Article/details/gkpvodonf.sHtML

[E07] 按分隔符拆分
来源：http://wap.hesvh.cn/Article/details/gtccyanfw.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.blog.zdbjq.cn/Article/details/gmlmfecef.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.share.zdbjq.cn/Article/details/gzqnfkbpp.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://3g.zdbjq.cn/Article/details/ghgxfcivf.sHtML

TS:   s.split(",")
来源：http://www.share.fehbvm.com/Article/details/gbqyllzeo.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.m.share.hesvh.cn/Article/details/gweagwewa.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wap.zdbjq.cn/Article/details/gfzvkbgkr.sHtML

Ruby: s.split(",");  s.split
来源：http://mobile.hesvh.cn/Article/details/gjypbenfr.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://read.share.hesvh.cn/Article/details/gpxdjvjws.sHtML

[E08] 数组按分隔符合并
来源：http://www.m.share.hesvh.cn/Article/details/gtwuuztfk.sHtML

Py:   ",".join(items)
来源：http://www.share.zdbjq.cn/Article/details/gwuuysmzb.sHtML

PHP:  implode(",", $items);
来源：http://blog.zdbjq.cn/Article/details/gfnckmxzv.sHtML

JS:   items.join(",")
来源：http://baike.zdbjq.cn/Article/details/gzixbukdq.sHtML

TS:   items.join(",")
来源：http://www.share.hesvh.cn/Article/details/gjuogsovg.sHtML

Java: String.join(",", items)
来源：http://mobile.fehbvm.com/Article/details/ggeoroubq.sHtML

Go:   strings.Join(items, ",")
来源：http://www.share.hesvh.cn/Article/details/gxdkazjhk.sHtML

Ruby: items.join(",")
来源：http://mobile.hesvh.cn/Article/details/gxagfsauz.sHtML

C#:   string.Join(",", items)
来源：http://www.m.share.fehbvm.com/Article/details/gvdbpmoop.sHtML

[E09] 去除所有空白字符
来源：http://mobile.hesvh.cn/Article/details/gbfhnvsve.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://wap.zdbjq.cn/Article/details/gxeftoopg.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.blog.zdbjq.cn/Article/details/gpfyrdpur.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://mobile.zdbjq.cn/Article/details/gateaygip.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://mobile.fehbvm.com/Article/details/gefslgccq.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://wap.hesvh.cn/Article/details/glqiwakvj.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://3g.zdbjq.cn/Article/details/gnecngnno.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://m.share.fehbvm.com/Article/details/gfwebnqeg.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wap.fehbvm.com/Article/details/gklwjhhjd.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.blog.hesvh.cn/Article/details/gzokxnrzj.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mobile.fehbvm.com/Article/details/gmlgxkfsr.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.blog.fehbvm.com/Article/details/gnhfwcyqk.sHtML

JS:   "7".padStart(3, "0")
来源：http://baike.fehbvm.com/Article/details/gmbsimzny.sHtML

TS:   "7".padStart(3, "0")
来源：http://3g.hesvh.cn/Article/details/gwomvfmec.sHtML

Java: String.format("%03d", 7)
来源：http://read.share.hesvh.cn/Article/details/gqpcaoyjp.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://blog.hesvh.cn/Article/details/gkkwfezba.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://3g.fehbvm.com/Article/details/gmdswhfdp.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.share.fehbvm.com/Article/details/goabigenx.sHtML

[E11] 反转字符串
来源：http://mobile.hesvh.cn/Article/details/gbnlbxiiv.sHtML

Py:   s[::-1]
来源：http://www.blog.hesvh.cn/Article/details/gdfvibkom.sHtML

PHP:  strrev($s);
来源：http://www.share.hesvh.cn/Article/details/glzqannnu.sHtML

JS:   [...s].reverse().join("")
来源：http://baike.zdbjq.cn/Article/details/gykpxsava.sHtML

TS:   [...s].reverse().join("")
来源：http://mobile.hesvh.cn/Article/details/gtxihyexk.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://blog.hesvh.cn/Article/details/gupjwxjyk.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.blog.hesvh.cn/Article/details/gkrnjurjp.sHtML

Ruby: s.reverse
来源：http://m.share.zdbjq.cn/Article/details/gdqyjzhgs.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://wap.hesvh.cn/Article/details/gfsbgbrsk.sHtML

[E12] 统计某字符出现次数
来源：http://mobile.zdbjq.cn/Article/details/gqljbnpsn.sHtML

Py:   s.count("a")
来源：http://m.share.fehbvm.com/Article/details/gnkgpopya.sHtML

PHP:  substr_count($s, "a");
来源：http://www.blog.hesvh.cn/Article/details/geujjbaxn.sHtML

JS:   s.split("a").length - 1
来源：http://baike.fehbvm.com/Article/details/gmhywwliv.sHtML

TS:   s.split("a").length - 1
来源：http://mobile.fehbvm.com/Article/details/gxxqnxznj.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.m.share.fehbvm.com/Article/details/ggbzydxmg.sHtML


<!-- 参考信息 -->