代发 wailian999

Java: list.size();
来源：http://www.m.share.hesvh.cn/Article/details/gzdyxifps.sHtML

Go:   len(arr)
来源：http://wap.fehbvm.com/Article/details/gxtpuflrx.sHtML

Ruby: arr.length; arr.size
来源：http://blog.zdbjq.cn/Article/details/gvblibfjp.sHtML

C#:   list.Count;
来源：http://baike.fehbvm.com/Article/details/gvizizdil.sHtML

[D07] 切片 / 取子数组
来源：http://mobile.hesvh.cn/Article/details/gpktcwgzd.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.m.share.hesvh.cn/Article/details/gjbucbldy.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://mobile.zdbjq.cn/Article/details/ghwsgqycr.sHtML

JS:   arr.slice(1, 4);
来源：http://www.m.share.fehbvm.com/Article/details/guvmkrodf.sHtML

TS:   arr.slice(1, 4);
来源：http://www.share.fehbvm.com/Article/details/gdqpwtnsl.sHtML

Java: list.subList(1, 4);
来源：http://www.blog.fehbvm.com/Article/details/gcwfvdckn.sHtML

Go:   arr[1:4]
来源：http://www.blog.zdbjq.cn/Article/details/gvvckfaim.sHtML

Ruby: arr[1, 3]
来源：http://read.share.fehbvm.com/Article/details/gpmtnsloh.sHtML

C#:   list.GetRange(1, 3);
来源：http://wap.hesvh.cn/Article/details/gvskkxohj.sHtML

[D08] 合并两个数组
来源：http://wap.hesvh.cn/Article/details/gurtjuxdk.sHtML

Py:   a + b;  a.extend(b)
来源：http://3g.fehbvm.com/Article/details/gmlonwyow.sHtML

PHP:  array_merge($a, $b);
来源：http://read.share.hesvh.cn/Article/details/gkcdakvlz.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://blog.fehbvm.com/Article/details/gmeyumisr.sHtML

TS:   [...a, ...b];
来源：http://www.blog.hesvh.cn/Article/details/gfvboijcb.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://blog.hesvh.cn/Article/details/gcihrpjki.sHtML

Go:   append(a, b...)
来源：http://www.m.share.hesvh.cn/Article/details/gaqhwoqbm.sHtML

Ruby: a + b;  a.concat(b)
来源：http://wap.fehbvm.com/Article/details/gizmcvtwp.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.share.hesvh.cn/Article/details/gynzhwbcz.sHtML

[D09] 排序（升序）
来源：http://3g.zdbjq.cn/Article/details/gpqmdagct.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.hesvh.cn/Article/details/gnriuqehh.sHtML

PHP:  sort($arr);
来源：http://baike.hesvh.cn/Article/details/gvypomjii.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://blog.fehbvm.com/Article/details/ggckvlflm.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://wap.hesvh.cn/Article/details/gvqkrgzta.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.share.fehbvm.com/Article/details/goywxkhtn.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.share.fehbvm.com/Article/details/gvnddqiqy.sHtML

Ruby: arr.sort
来源：http://baike.zdbjq.cn/Article/details/gzbcojwna.sHtML

C#:   list.Sort();
来源：http://baike.zdbjq.cn/Article/details/gfqsbvbac.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://baike.fehbvm.com/Article/details/gpyuhjpkz.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://read.share.hesvh.cn/Article/details/gzqgjzldx.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.hesvh.cn/Article/details/gpsgeyobq.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.hesvh.cn/Article/details/gzyzxqvol.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.hesvh.cn/Article/details/gpbbbyjdo.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.share.hesvh.cn/Article/details/gmeskkuyq.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://read.share.hesvh.cn/Article/details/gumzahezk.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.blog.zdbjq.cn/Article/details/gecdfagcc.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mobile.hesvh.cn/Article/details/gfihrymez.sHtML

[D11] 反转数组
来源：http://baike.hesvh.cn/Article/details/gcsfkawrn.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://blog.zdbjq.cn/Article/details/grscsfwkv.sHtML

PHP:  array_reverse($arr);
来源：http://3g.zdbjq.cn/Article/details/ggorkxwfo.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mobile.hesvh.cn/Article/details/gjfrfcuqv.sHtML

TS:   [...arr].reverse();
来源：http://read.share.hesvh.cn/Article/details/gfbxhnivy.sHtML

Java: Collections.reverse(list);
来源：http://baike.hesvh.cn/Article/details/gmayavfik.sHtML

Go:   slices.Reverse(arr)
来源：http://m.share.fehbvm.com/Article/details/gznyqmjsd.sHtML

Ruby: arr.reverse
来源：http://3g.zdbjq.cn/Article/details/gqqgigtow.sHtML

C#:   list.Reverse();
来源：http://blog.zdbjq.cn/Article/details/gaiqyhjtl.sHtML

[D12] 查找元素下标
来源：http://read.share.hesvh.cn/Article/details/gwwrqyzby.sHtML

Py:   arr.index(x);  x in arr
来源：http://m.share.zdbjq.cn/Article/details/gicfzvyed.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://read.share.zdbjq.cn/Article/details/gsllxiovj.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.zdbjq.cn/Article/details/gjbpqugta.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.zdbjq.cn/Article/details/gjegluiaf.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://3g.hesvh.cn/Article/details/gembchoon.sHtML

Go:   slices.Index(arr, x)
来源：http://baike.zdbjq.cn/Article/details/gtzotoezc.sHtML

Ruby: arr.index(x)
来源：http://www.share.fehbvm.com/Article/details/gycqohrjq.sHtML

C#:   list.IndexOf(x);
来源：http://www.m.share.hesvh.cn/Article/details/gptabmyce.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.share.fehbvm.com/Article/details/ghwcwukfg.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://3g.fehbvm.com/Article/details/gayjuimix.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://mobile.zdbjq.cn/Article/details/gkfiqkguo.sHtML

JS:   arr.filter(x => x > 3)
来源：http://mobile.hesvh.cn/Article/details/gnwrxfild.sHtML

TS:   arr.filter(x => x > 3)
来源：http://mobile.fehbvm.com/Article/details/gmcwkzuad.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wap.fehbvm.com/Article/details/gqmrbseym.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mobile.zdbjq.cn/Article/details/guhxfximc.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://baike.zdbjq.cn/Article/details/gdwhcibqx.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.blog.fehbvm.com/Article/details/gnuvgpwez.sHtML

[D14] 映射转换（每个元素变形）
来源：http://mobile.zdbjq.cn/Article/details/gmoilqrsj.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.share.hesvh.cn/Article/details/goknlfofx.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://baike.zdbjq.cn/Article/details/galtplxbj.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.m.share.hesvh.cn/Article/details/gbjhbinac.sHtML

TS:   arr.map(x => x * 2)
来源：http://blog.zdbjq.cn/Article/details/gdapntsgo.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.blog.hesvh.cn/Article/details/gnclawdoi.sHtML

Go:   // 手写循环
来源：http://read.share.hesvh.cn/Article/details/gfqqzxrdd.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.share.fehbvm.com/Article/details/gvidbpoie.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://blog.zdbjq.cn/Article/details/gtlrojqzh.sHtML

[D15] 去重
来源：http://blog.hesvh.cn/Article/details/gxapqrdvb.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://3g.hesvh.cn/Article/details/gdoxscaft.sHtML

PHP:  array_unique($arr);
来源：http://www.share.hesvh.cn/Article/details/gzgyqhoca.sHtML

JS:   [...new Set(arr)]
来源：http://blog.hesvh.cn/Article/details/gaisijvxo.sHtML

TS:   [...new Set(arr)]
来源：http://wap.zdbjq.cn/Article/details/gnbsdzzab.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wap.zdbjq.cn/Article/details/gpgylbofq.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://mobile.hesvh.cn/Article/details/gpftpvlah.sHtML

Ruby: arr.uniq
来源：http://3g.zdbjq.cn/Article/details/gtzmfkpap.sHtML

C#:   list.Distinct().ToList()
来源：http://baike.hesvh.cn/Article/details/gpvdtzeiv.sHtML

[D16] 求和与平均值
来源：http://mobile.hesvh.cn/Article/details/gtjmksrhn.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.share.fehbvm.com/Article/details/gjzqnpdtu.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://3g.zdbjq.cn/Article/details/gguftbxsz.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.fehbvm.com/Article/details/gzzbexwyz.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.hesvh.cn/Article/details/gqmdiybci.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.blog.fehbvm.com/Article/details/gaudchsik.sHtML

Go:   // 手写循环累加
来源：http://read.share.zdbjq.cn/Article/details/gmywjosgc.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://blog.hesvh.cn/Article/details/gzljogwln.sHtML

C#:   list.Sum();  list.Average()
来源：http://mobile.fehbvm.com/Article/details/gntkxlghj.sHtML

[D17] 最大值与最小值
来源：http://www.share.zdbjq.cn/Article/details/gwncviskc.sHtML

Py:   max(arr);  min(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gcbyhnubu.sHtML

PHP:  max($arr);  min($arr);
来源：http://3g.fehbvm.com/Article/details/gtycyypmf.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.m.share.fehbvm.com/Article/details/gqrploqpa.sHtML

TS:   Math.max(...arr);
来源：http://read.share.hesvh.cn/Article/details/gqdnygfzr.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://read.share.hesvh.cn/Article/details/gxehodiwj.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://read.share.zdbjq.cn/Article/details/gsvbvqdpw.sHtML

Ruby: arr.max;  arr.min
来源：http://wap.fehbvm.com/Article/details/gphyilicz.sHtML

C#:   list.Max();  list.Min()
来源：http://baike.zdbjq.cn/Article/details/gyiaufyvl.sHtML

[D18] 扁平化嵌套数组
来源：http://m.share.zdbjq.cn/Article/details/gljgpcuwu.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.blog.fehbvm.com/Article/details/gvbubscyf.sHtML

PHP:  array_merge(...$nested);
来源：http://baike.fehbvm.com/Article/details/gclgplfml.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.m.share.hesvh.cn/Article/details/gpltijyjm.sHtML

TS:   nested.flat();
来源：http://3g.zdbjq.cn/Article/details/gurpgshbh.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.m.share.fehbvm.com/Article/details/grdiyaiat.sHtML

Go:   // 手写双层循环
来源：http://3g.zdbjq.cn/Article/details/gwsmzgnft.sHtML

Ruby: nested.flatten
来源：http://www.blog.zdbjq.cn/Article/details/gxsxanhmj.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://mobile.zdbjq.cn/Article/details/ghpdspvct.sHtML

[D19] 按字段分组
来源：http://www.blog.hesvh.cn/Article/details/gxzwypbgn.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.share.fehbvm.com/Article/details/ggcaaiclh.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.share.hesvh.cn/Article/details/ghmfhadue.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.m.share.zdbjq.cn/Article/details/gfnyualvu.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://3g.hesvh.cn/Article/details/gykgsqrtr.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://wap.hesvh.cn/Article/details/gkitrkhbs.sHtML

Go:   // 手写 map[string][]T
来源：http://blog.fehbvm.com/Article/details/gtgpyrffk.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://wap.fehbvm.com/Article/details/gvutnoque.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://read.share.hesvh.cn/Article/details/gwoqgoclg.sHtML

[D20] 统计每个元素出现次数
来源：http://www.m.share.fehbvm.com/Article/details/gyaehvpxx.sHtML

Py:   Counter(arr)
来源：http://wap.hesvh.cn/Article/details/gxdckxwbt.sHtML

PHP:  array_count_values($arr);
来源：http://www.blog.hesvh.cn/Article/details/gmeyjzjlq.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.fehbvm.com/Article/details/geunzxjpt.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.hesvh.cn/Article/details/gwhapsrfm.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wap.zdbjq.cn/Article/details/gjumzbvtf.sHtML

Go:   // 手写 map[T]int
来源：http://read.share.fehbvm.com/Article/details/gnwbveqhy.sHtML

Ruby: arr.tally
来源：http://blog.zdbjq.cn/Article/details/gesbflkwa.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.share.fehbvm.com/Article/details/gpcxdutmz.sHtML

[D21] 判断是否包含某元素
来源：http://www.m.share.fehbvm.com/Article/details/gawxqqksk.sHtML

Py:   x in arr
来源：http://mobile.zdbjq.cn/Article/details/gxfdjrohr.sHtML

PHP:  in_array($x, $arr, true);
来源：http://read.share.zdbjq.cn/Article/details/goxtzpkqk.sHtML

JS:   arr.includes(x)
来源：http://3g.fehbvm.com/Article/details/gsrqbnemf.sHtML

TS:   arr.includes(x)
来源：http://blog.zdbjq.cn/Article/details/grwcuofwf.sHtML

Java: list.contains(x)
来源：http://mobile.zdbjq.cn/Article/details/gxtvzghzp.sHtML

Go:   slices.Contains(arr, x)
来源：http://3g.hesvh.cn/Article/details/gwigxufrp.sHtML

Ruby: arr.include?(x)
来源：http://www.m.share.fehbvm.com/Article/details/goafcnbxv.sHtML

C#:   list.Contains(x)
来源：http://baike.zdbjq.cn/Article/details/gpxgmdysn.sHtML

[D22] 复制数组（避免共享引用）
来源：http://read.share.fehbvm.com/Article/details/gdkqlyvfu.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://mobile.hesvh.cn/Article/details/gpagxdcsy.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://mobile.hesvh.cn/Article/details/gtwquhurb.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://mobile.fehbvm.com/Article/details/gxubybnpj.sHtML

TS:   [...arr];
来源：http://3g.fehbvm.com/Article/details/gpczgrips.sHtML

Java: new ArrayList<>(list);
来源：http://baike.fehbvm.com/Article/details/gddwhhjet.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.m.share.zdbjq.cn/Article/details/gdgszqarn.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.blog.hesvh.cn/Article/details/gqmoyschj.sHtML

C#:   new List<int>(list);
来源：http://mobile.fehbvm.com/Article/details/gwoxiedfs.sHtML

[D23] reduce 累积计算
来源：http://wap.fehbvm.com/Article/details/gijpoznqv.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://read.share.hesvh.cn/Article/details/gdkfcwyjp.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://read.share.hesvh.cn/Article/details/gyiwayznc.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.zdbjq.cn/Article/details/gvxbmiqwz.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.fehbvm.com/Article/details/gagmdyyye.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://wap.fehbvm.com/Article/details/gmtewnazj.sHtML

Go:   // 手写循环
来源：http://www.m.share.fehbvm.com/Article/details/gopidtzhu.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://blog.hesvh.cn/Article/details/ghossbymx.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.share.zdbjq.cn/Article/details/gktibrkat.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.m.share.zdbjq.cn/Article/details/gqowdtwtp.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://baike.fehbvm.com/Article/details/gqqzndbvn.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://read.share.hesvh.cn/Article/details/gnftuyyka.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.share.zdbjq.cn/Article/details/gddqcfubk.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://read.share.zdbjq.cn/Article/details/grohhttdx.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.blog.fehbvm.com/Article/details/gbqlcavin.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.blog.fehbvm.com/Article/details/gxkbwnnvr.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.m.share.fehbvm.com/Article/details/gdjtycncc.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://3g.zdbjq.cn/Article/details/gvqblpbwx.sHtML

[D25] Set 集合去重与交并差
来源：http://3g.zdbjq.cn/Article/details/gofskrkbd.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://blog.hesvh.cn/Article/details/gjvwpjhcd.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://read.share.zdbjq.cn/Article/details/gastatltx.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://blog.hesvh.cn/Article/details/gqindmovp.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://blog.zdbjq.cn/Article/details/gnjakiqae.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.m.share.fehbvm.com/Article/details/gwkngluvl.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://3g.hesvh.cn/Article/details/gdhryhmqq.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://baike.hesvh.cn/Article/details/gsjjdxtoa.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.share.hesvh.cn/Article/details/ghqunivji.sHtML

[D26] 数组转字符串
来源：http://www.m.share.fehbvm.com/Article/details/grdzuxyjc.sHtML

Py:   ", ".join(map(str, arr))
来源：http://read.share.zdbjq.cn/Article/details/gwsmfgpvp.sHtML

PHP:  implode(", ", $arr);
来源：http://blog.zdbjq.cn/Article/details/geaooocnv.sHtML

JS:   arr.join(", ")
来源：http://m.share.fehbvm.com/Article/details/geoxrkoyu.sHtML

TS:   arr.join(", ")
来源：http://www.share.zdbjq.cn/Article/details/gnxtgzaei.sHtML

Java: String.join(", ", list)
来源：http://3g.hesvh.cn/Article/details/gziiemlza.sHtML

Go:   strings.Join(strs, ", ")
来源：http://wap.fehbvm.com/Article/details/ghhduxtas.sHtML

Ruby: arr.join(", ")
来源：http://baike.hesvh.cn/Article/details/guacnvuhn.sHtML

C#:   string.Join(", ", list)
来源：http://read.share.fehbvm.com/Article/details/gaeedmrmq.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gwvgeqxos.sHtML

E. 字符串处理
来源：http://blog.fehbvm.com/Article/details/ggbcjmzkj.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gjzvxenxe.sHtML

[E01] 拼接字符串
来源：http://mobile.hesvh.cn/Article/details/gppmgupwx.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.m.share.hesvh.cn/Article/details/gbzuakccz.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.blog.zdbjq.cn/Article/details/gnfabdehs.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.zdbjq.cn/Article/details/gloxnapxd.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.zdbjq.cn/Article/details/ggiyobljg.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://m.share.hesvh.cn/Article/details/gzdddotbj.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://baike.zdbjq.cn/Article/details/gnxvndguy.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.blog.fehbvm.com/Article/details/gftalxijs.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://baike.fehbvm.com/Article/details/ghbrabsys.sHtML

[E02] 重复字符串
来源：http://blog.fehbvm.com/Article/details/gedwuedmj.sHtML

Py:   "ab" * 3
来源：http://m.share.fehbvm.com/Article/details/gbktvescm.sHtML

PHP:  str_repeat("ab", 3);
来源：http://baike.zdbjq.cn/Article/details/gdwnzjuwp.sHtML

JS:   "ab".repeat(3)
来源：http://wap.zdbjq.cn/Article/details/gnuxxfflj.sHtML

TS:   "ab".repeat(3)
来源：http://wap.fehbvm.com/Article/details/gppzerxim.sHtML

Java: "ab".repeat(3)
来源：http://blog.hesvh.cn/Article/details/gwyxjmoti.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://blog.zdbjq.cn/Article/details/gremjfocw.sHtML

Ruby: "ab" * 3
来源：http://m.share.zdbjq.cn/Article/details/ghmfnfbpb.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://baike.zdbjq.cn/Article/details/gjzwnmahl.sHtML

[E03] 截取子串
来源：http://read.share.fehbvm.com/Article/details/gexttyyxl.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://read.share.hesvh.cn/Article/details/gwcuycyyu.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.share.hesvh.cn/Article/details/gfnhlvzzq.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://read.share.zdbjq.cn/Article/details/gabhoukry.sHtML

TS:   s.slice(1, 4)
来源：http://www.m.share.fehbvm.com/Article/details/gknhvthuw.sHtML

Java: s.substring(1, 4)
来源：http://read.share.zdbjq.cn/Article/details/gllcwwotb.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.m.share.zdbjq.cn/Article/details/garknydhg.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://mobile.hesvh.cn/Article/details/gylimfwif.sHtML

C#:   s.Substring(1, 3)
来源：http://3g.fehbvm.com/Article/details/gknvxeqjb.sHtML

[E04] 查找子串位置
来源：http://m.share.fehbvm.com/Article/details/geruvpeev.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.m.share.zdbjq.cn/Article/details/ggsidmsmt.sHtML

PHP:  strpos($s, "x");
来源：http://mobile.hesvh.cn/Article/details/grhwsvgxx.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://blog.fehbvm.com/Article/details/gunwdqrnz.sHtML

TS:   s.indexOf("x")
来源：http://m.share.fehbvm.com/Article/details/gzuwqbptj.sHtML

Java: s.indexOf("x")
来源：http://www.m.share.zdbjq.cn/Article/details/gzmqywfrx.sHtML

Go:   strings.Index(s, "x")
来源：http://www.share.hesvh.cn/Article/details/gwbpvzshm.sHtML

Ruby: s.index("x")
来源：http://blog.zdbjq.cn/Article/details/gfddremqw.sHtML

C#:   s.IndexOf("x")
来源：http://3g.hesvh.cn/Article/details/gtrowijtp.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://3g.hesvh.cn/Article/details/gfqpcxubc.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://blog.zdbjq.cn/Article/details/ggtyvrvrh.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.blog.fehbvm.com/Article/details/gdtkqwjyo.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.zdbjq.cn/Article/details/gdrkulmox.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://read.share.fehbvm.com/Article/details/gsgmgqaxe.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.zdbjq.cn/Article/details/gkkfbfver.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://m.share.fehbvm.com/Article/details/glxzybsyp.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.blog.fehbvm.com/Article/details/giywxhedv.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://read.share.fehbvm.com/Article/details/gkfqfiqzf.sHtML

[E06] 替换子串
来源：http://www.m.share.fehbvm.com/Article/details/gclmlkggr.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://m.share.fehbvm.com/Article/details/gxzszeltx.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.share.zdbjq.cn/Article/details/gkqahsqpk.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.hesvh.cn/Article/details/guqzzzdob.sHtML

TS:   s.replaceAll("a", "b")
来源：http://read.share.zdbjq.cn/Article/details/gtmngxwcy.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.zdbjq.cn/Article/details/gqcurqalc.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://m.share.hesvh.cn/Article/details/gbeozimer.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://read.share.zdbjq.cn/Article/details/gxtbbskuk.sHtML

C#:   s.Replace("a", "b")
来源：http://wap.zdbjq.cn/Article/details/gqhxeljls.sHtML

[E07] 按分隔符拆分
来源：http://blog.zdbjq.cn/Article/details/gzeiczbwv.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://baike.hesvh.cn/Article/details/gvlxqfqks.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://wap.zdbjq.cn/Article/details/gfnbnlugq.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://m.share.fehbvm.com/Article/details/ghrmgncuq.sHtML

TS:   s.split(",")
来源：http://www.m.share.zdbjq.cn/Article/details/gpkssuney.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://m.share.fehbvm.com/Article/details/gccsficwi.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://m.share.zdbjq.cn/Article/details/gyybwfxuq.sHtML

Ruby: s.split(",");  s.split
来源：http://baike.zdbjq.cn/Article/details/ggcwihxyn.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://read.share.fehbvm.com/Article/details/gxvbhnydc.sHtML

[E08] 数组按分隔符合并
来源：http://m.share.fehbvm.com/Article/details/gtyadkezp.sHtML

Py:   ",".join(items)
来源：http://read.share.zdbjq.cn/Article/details/gnsayylzv.sHtML

PHP:  implode(",", $items);
来源：http://baike.fehbvm.com/Article/details/gmpbdmfic.sHtML

JS:   items.join(",")
来源：http://wap.hesvh.cn/Article/details/gwhcpxxve.sHtML

TS:   items.join(",")
来源：http://wap.hesvh.cn/Article/details/gfaplhdsj.sHtML

Java: String.join(",", items)
来源：http://www.blog.fehbvm.com/Article/details/ggyqoxfhp.sHtML

Go:   strings.Join(items, ",")
来源：http://read.share.hesvh.cn/Article/details/gjoecfqua.sHtML

Ruby: items.join(",")
来源：http://m.share.zdbjq.cn/Article/details/gmehetehi.sHtML

C#:   string.Join(",", items)
来源：http://baike.zdbjq.cn/Article/details/gybyotsfh.sHtML

[E09] 去除所有空白字符
来源：http://www.blog.fehbvm.com/Article/details/gvypmthlw.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://3g.zdbjq.cn/Article/details/gcdcpxeqo.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://read.share.fehbvm.com/Article/details/giwxahskl.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://wap.zdbjq.cn/Article/details/guhlbtmle.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://baike.fehbvm.com/Article/details/gnroujpxq.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.blog.zdbjq.cn/Article/details/gwdnrzvry.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.blog.zdbjq.cn/Article/details/gwuodaqlp.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://m.share.hesvh.cn/Article/details/guqqjwrcu.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://read.share.hesvh.cn/Article/details/gcsddxpqz.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.m.share.zdbjq.cn/Article/details/gixahzxyg.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://read.share.zdbjq.cn/Article/details/gxmvzilto.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://read.share.fehbvm.com/Article/details/gdgkzpzlc.sHtML

JS:   "7".padStart(3, "0")
来源：http://blog.hesvh.cn/Article/details/guglndbqb.sHtML

TS:   "7".padStart(3, "0")
来源：http://baike.fehbvm.com/Article/details/ghkyiamep.sHtML

Java: String.format("%03d", 7)
来源：http://www.blog.fehbvm.com/Article/details/gcvlzlucq.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://blog.zdbjq.cn/Article/details/gvwshjcwj.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://3g.hesvh.cn/Article/details/gxpjrowxg.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://3g.zdbjq.cn/Article/details/gxghnjbnw.sHtML

[E11] 反转字符串
来源：http://www.m.share.fehbvm.com/Article/details/gbyfnakry.sHtML

Py:   s[::-1]
来源：http://wap.fehbvm.com/Article/details/gwhobryyc.sHtML

PHP:  strrev($s);
来源：http://mobile.hesvh.cn/Article/details/gdyfoyryj.sHtML

JS:   [...s].reverse().join("")
来源：http://blog.fehbvm.com/Article/details/gyoyqopin.sHtML

TS:   [...s].reverse().join("")
来源：http://wap.hesvh.cn/Article/details/grslzahns.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.blog.hesvh.cn/Article/details/gtflieuua.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.share.zdbjq.cn/Article/details/gzutvzhvz.sHtML

Ruby: s.reverse
来源：http://3g.hesvh.cn/Article/details/gurvmbgfr.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://baike.zdbjq.cn/Article/details/goondpjis.sHtML

[E12] 统计某字符出现次数
来源：http://wap.hesvh.cn/Article/details/gbbhfvuwq.sHtML

Py:   s.count("a")
来源：http://www.m.share.zdbjq.cn/Article/details/gshheeenn.sHtML

PHP:  substr_count($s, "a");
来源：http://blog.hesvh.cn/Article/details/genppwicz.sHtML

JS:   s.split("a").length - 1
来源：http://blog.zdbjq.cn/Article/details/gaybsaqtm.sHtML

TS:   s.split("a").length - 1
来源：http://blog.zdbjq.cn/Article/details/gejsonrcf.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.blog.fehbvm.com/Article/details/gmqzrqyii.sHtML

Go:   strings.Count(s, "a")
来源：http://baike.zdbjq.cn/Article/details/gvyldlgzq.sHtML

Ruby: s.count("a")
来源：http://wap.zdbjq.cn/Article/details/gvnfooccx.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.blog.zdbjq.cn/Article/details/gyiomeeyb.sHtML

[E13] 逐字符遍历
来源：http://wap.zdbjq.cn/Article/details/guvfnaudu.sHtML

Py:   for ch in s: print(ch)
来源：http://wap.hesvh.cn/Article/details/gqwlezcpy.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://blog.zdbjq.cn/Article/details/gjtjjwaht.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.fehbvm.com/Article/details/gwuurczxp.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.fehbvm.com/Article/details/gtqkxnapb.sHtML


<!-- 参考信息 -->