代发 wailian999

Ruby: a + b;  a.concat(b)
来源：http://read.share.fehbvm.com/Article/details/gfnvqeffr.sHtML

C#:   a.Concat(b).ToList()
来源：http://wap.hesvh.cn/Article/details/ghxuvanrg.sHtML

[D09] 排序（升序）
来源：http://m.share.fehbvm.com/Article/details/gdikuopue.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.hesvh.cn/Article/details/gmapheprw.sHtML

PHP:  sort($arr);
来源：http://www.blog.zdbjq.cn/Article/details/gwjbcoojt.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://m.share.zdbjq.cn/Article/details/gbxfjdghm.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://read.share.hesvh.cn/Article/details/gkeqeuchq.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://mobile.fehbvm.com/Article/details/gqjzlrqam.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://3g.zdbjq.cn/Article/details/glorbomsu.sHtML

Ruby: arr.sort
来源：http://wap.fehbvm.com/Article/details/gzrfkwgcs.sHtML

C#:   list.Sort();
来源：http://www.m.share.fehbvm.com/Article/details/giejenrkr.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://baike.hesvh.cn/Article/details/gwsliadbq.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://m.share.zdbjq.cn/Article/details/gjczjptnw.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.fehbvm.com/Article/details/ghaquwlce.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.hesvh.cn/Article/details/gywstlokn.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.fehbvm.com/Article/details/gmgsaqhqf.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://3g.fehbvm.com/Article/details/gcxqhteos.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.blog.fehbvm.com/Article/details/gvtmemqwj.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://m.share.zdbjq.cn/Article/details/grictkall.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.m.share.zdbjq.cn/Article/details/gaeanpdse.sHtML

[D11] 反转数组
来源：http://baike.fehbvm.com/Article/details/gwdofrqvd.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://m.share.hesvh.cn/Article/details/gxcwvabbh.sHtML

PHP:  array_reverse($arr);
来源：http://baike.hesvh.cn/Article/details/gvckpnjmo.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://baike.hesvh.cn/Article/details/gcvkdvvcj.sHtML

TS:   [...arr].reverse();
来源：http://read.share.fehbvm.com/Article/details/gfbsxkktn.sHtML

Java: Collections.reverse(list);
来源：http://www.blog.fehbvm.com/Article/details/gzpllhtog.sHtML

Go:   slices.Reverse(arr)
来源：http://m.share.hesvh.cn/Article/details/gnsapijch.sHtML

Ruby: arr.reverse
来源：http://read.share.fehbvm.com/Article/details/ghevstzcu.sHtML

C#:   list.Reverse();
来源：http://blog.hesvh.cn/Article/details/gmfcgotjg.sHtML

[D12] 查找元素下标
来源：http://3g.fehbvm.com/Article/details/gfeytsitq.sHtML

Py:   arr.index(x);  x in arr
来源：http://blog.zdbjq.cn/Article/details/gvfowmewi.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://read.share.hesvh.cn/Article/details/getoxkyjx.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.hesvh.cn/Article/details/gvjkikcve.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.hesvh.cn/Article/details/gkaizojht.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://mobile.hesvh.cn/Article/details/gkymasmko.sHtML

Go:   slices.Index(arr, x)
来源：http://mobile.hesvh.cn/Article/details/gpvgnryse.sHtML

Ruby: arr.index(x)
来源：http://www.blog.zdbjq.cn/Article/details/gkissdcyt.sHtML

C#:   list.IndexOf(x);
来源：http://wap.fehbvm.com/Article/details/gbdlsxlpq.sHtML

[D13] 过滤（保留满足条件的）
来源：http://3g.fehbvm.com/Article/details/gfjvtbnsi.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://blog.hesvh.cn/Article/details/gzuhnkzvv.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://blog.hesvh.cn/Article/details/gnshdrtwq.sHtML

JS:   arr.filter(x => x > 3)
来源：http://read.share.hesvh.cn/Article/details/grwlxmfjw.sHtML

TS:   arr.filter(x => x > 3)
来源：http://3g.hesvh.cn/Article/details/gcbfjcdpl.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://blog.hesvh.cn/Article/details/gcrosovgp.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mobile.hesvh.cn/Article/details/gllllhxiq.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://mobile.hesvh.cn/Article/details/gfsgystaq.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://blog.zdbjq.cn/Article/details/gsggviwfc.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.m.share.hesvh.cn/Article/details/gqijhtvve.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.blog.fehbvm.com/Article/details/gbctbxvuq.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://blog.hesvh.cn/Article/details/gaoqtljwm.sHtML

JS:   arr.map(x => x * 2)
来源：http://3g.zdbjq.cn/Article/details/gthydfwav.sHtML

TS:   arr.map(x => x * 2)
来源：http://read.share.hesvh.cn/Article/details/gqifcncrt.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://3g.zdbjq.cn/Article/details/grszxhzme.sHtML

Go:   // 手写循环
来源：http://mobile.zdbjq.cn/Article/details/gprnaesil.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://blog.fehbvm.com/Article/details/gmxqoutyp.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://baike.hesvh.cn/Article/details/gomztpbyh.sHtML

[D15] 去重
来源：http://read.share.zdbjq.cn/Article/details/gcildtrhg.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://blog.hesvh.cn/Article/details/gqtxcxafc.sHtML

PHP:  array_unique($arr);
来源：http://blog.fehbvm.com/Article/details/gtfdthzpk.sHtML

JS:   [...new Set(arr)]
来源：http://www.blog.hesvh.cn/Article/details/gqwxokylh.sHtML

TS:   [...new Set(arr)]
来源：http://baike.zdbjq.cn/Article/details/grwgvnrbv.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.blog.hesvh.cn/Article/details/gzlugoemf.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.m.share.hesvh.cn/Article/details/giwubyimm.sHtML

Ruby: arr.uniq
来源：http://www.blog.zdbjq.cn/Article/details/gsfhbevrd.sHtML

C#:   list.Distinct().ToList()
来源：http://baike.fehbvm.com/Article/details/geyuasygb.sHtML

[D16] 求和与平均值
来源：http://www.share.hesvh.cn/Article/details/gfrckmhis.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://mobile.zdbjq.cn/Article/details/gcnuatxnz.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://read.share.zdbjq.cn/Article/details/gpxptyzds.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.fehbvm.com/Article/details/gufkfihjn.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.zdbjq.cn/Article/details/gyvmbvmqp.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://read.share.fehbvm.com/Article/details/gtncgtloq.sHtML

Go:   // 手写循环累加
来源：http://wap.zdbjq.cn/Article/details/givhxwxzc.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://m.share.fehbvm.com/Article/details/gtkvubpof.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.share.hesvh.cn/Article/details/gctdvbnvf.sHtML

[D17] 最大值与最小值
来源：http://www.share.zdbjq.cn/Article/details/guchehvpn.sHtML

Py:   max(arr);  min(arr)
来源：http://read.share.hesvh.cn/Article/details/gtvgogdpc.sHtML

PHP:  max($arr);  min($arr);
来源：http://m.share.fehbvm.com/Article/details/gtxocowny.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://3g.zdbjq.cn/Article/details/gbodyxpol.sHtML

TS:   Math.max(...arr);
来源：http://baike.hesvh.cn/Article/details/glqduvcor.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.m.share.fehbvm.com/Article/details/goosykhum.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.m.share.hesvh.cn/Article/details/geobbfomz.sHtML

Ruby: arr.max;  arr.min
来源：http://wap.fehbvm.com/Article/details/gocxdfcsd.sHtML

C#:   list.Max();  list.Min()
来源：http://www.share.zdbjq.cn/Article/details/gbwmxcklg.sHtML

[D18] 扁平化嵌套数组
来源：http://m.share.fehbvm.com/Article/details/gygcnsfbf.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.m.share.zdbjq.cn/Article/details/govbpgmrn.sHtML

PHP:  array_merge(...$nested);
来源：http://blog.zdbjq.cn/Article/details/glwucoxld.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://baike.zdbjq.cn/Article/details/gncqvriee.sHtML

TS:   nested.flat();
来源：http://3g.zdbjq.cn/Article/details/garphzcxv.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wap.fehbvm.com/Article/details/gvxuvewkh.sHtML

Go:   // 手写双层循环
来源：http://blog.hesvh.cn/Article/details/gstdnbbym.sHtML

Ruby: nested.flatten
来源：http://wap.zdbjq.cn/Article/details/gltsilpyl.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://3g.fehbvm.com/Article/details/gjzwmkjab.sHtML

[D19] 按字段分组
来源：http://www.share.zdbjq.cn/Article/details/gajqusvis.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://blog.hesvh.cn/Article/details/geddnbewe.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wap.zdbjq.cn/Article/details/gmdcraodn.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://3g.zdbjq.cn/Article/details/gbffkyygc.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://m.share.fehbvm.com/Article/details/ghkcmobdw.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.blog.zdbjq.cn/Article/details/glsiygjmp.sHtML

Go:   // 手写 map[string][]T
来源：http://read.share.fehbvm.com/Article/details/gyosehmfr.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://m.share.hesvh.cn/Article/details/gnlenlnok.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.share.zdbjq.cn/Article/details/gzlraccer.sHtML

[D20] 统计每个元素出现次数
来源：http://www.share.fehbvm.com/Article/details/gftpyitzx.sHtML

Py:   Counter(arr)
来源：http://blog.zdbjq.cn/Article/details/grgwudnjx.sHtML

PHP:  array_count_values($arr);
来源：http://www.share.hesvh.cn/Article/details/gfondlotf.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.fehbvm.com/Article/details/gocrqjsol.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.hesvh.cn/Article/details/gevrzptob.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://blog.fehbvm.com/Article/details/gzoyzjvdf.sHtML

Go:   // 手写 map[T]int
来源：http://3g.fehbvm.com/Article/details/gofyzwcjd.sHtML

Ruby: arr.tally
来源：http://m.share.hesvh.cn/Article/details/gdpaenakh.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://blog.zdbjq.cn/Article/details/gwhdobaah.sHtML

[D21] 判断是否包含某元素
来源：http://mobile.fehbvm.com/Article/details/gbkngqzbj.sHtML

Py:   x in arr
来源：http://3g.zdbjq.cn/Article/details/gtfpqhnqh.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.m.share.hesvh.cn/Article/details/gnmxrwisy.sHtML

JS:   arr.includes(x)
来源：http://wap.hesvh.cn/Article/details/giqgszvyq.sHtML

TS:   arr.includes(x)
来源：http://wap.fehbvm.com/Article/details/glvsrdtbj.sHtML

Java: list.contains(x)
来源：http://www.m.share.fehbvm.com/Article/details/ggrvoakdg.sHtML

Go:   slices.Contains(arr, x)
来源：http://blog.hesvh.cn/Article/details/gqixwittr.sHtML

Ruby: arr.include?(x)
来源：http://m.share.zdbjq.cn/Article/details/gifzbmtie.sHtML

C#:   list.Contains(x)
来源：http://wap.hesvh.cn/Article/details/gwjyconek.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.m.share.fehbvm.com/Article/details/ghlppmwhx.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gwcybehwy.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://m.share.zdbjq.cn/Article/details/gjxwrxwod.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://read.share.fehbvm.com/Article/details/gjtiunawv.sHtML

TS:   [...arr];
来源：http://www.share.fehbvm.com/Article/details/gwzwzlgsf.sHtML

Java: new ArrayList<>(list);
来源：http://read.share.hesvh.cn/Article/details/gohtqxbyg.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.share.hesvh.cn/Article/details/gtwcbvvxq.sHtML

Ruby: arr.dup;  arr.clone
来源：http://read.share.hesvh.cn/Article/details/ggcqrrsnq.sHtML

C#:   new List<int>(list);
来源：http://www.blog.fehbvm.com/Article/details/gekoosnrq.sHtML

[D23] reduce 累积计算
来源：http://blog.zdbjq.cn/Article/details/guhbdhakz.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://baike.zdbjq.cn/Article/details/gvrzegijc.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://read.share.fehbvm.com/Article/details/gscizrmbq.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/gbagsgqmq.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.hesvh.cn/Article/details/gkebqlywz.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.blog.zdbjq.cn/Article/details/gwxfazbis.sHtML

Go:   // 手写循环
来源：http://wap.zdbjq.cn/Article/details/gghirxqng.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://read.share.hesvh.cn/Article/details/gcabtlupw.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.m.share.zdbjq.cn/Article/details/gdasvqjlj.sHtML

[D24] 字典 / Map 基本操作
来源：http://3g.hesvh.cn/Article/details/gudlnnvrq.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wap.zdbjq.cn/Article/details/gtezktgvs.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://baike.fehbvm.com/Article/details/gdjvmxwlj.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://m.share.hesvh.cn/Article/details/gsbzvjpuh.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.blog.zdbjq.cn/Article/details/gognyqlgb.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://m.share.hesvh.cn/Article/details/grfsufyvs.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.m.share.hesvh.cn/Article/details/gwfvyarue.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.share.hesvh.cn/Article/details/gkvewqewj.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://baike.fehbvm.com/Article/details/glhhvrfjj.sHtML

[D25] Set 集合去重与交并差
来源：http://3g.zdbjq.cn/Article/details/gwhxutvvj.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://read.share.fehbvm.com/Article/details/gtvjtptpm.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.m.share.zdbjq.cn/Article/details/gfimrqnrr.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://read.share.fehbvm.com/Article/details/gmfrfmldx.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.m.share.zdbjq.cn/Article/details/gpbaaiqap.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://3g.hesvh.cn/Article/details/gasmamfpe.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://baike.zdbjq.cn/Article/details/gtpefzhco.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://read.share.zdbjq.cn/Article/details/gqwfaaghu.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://blog.zdbjq.cn/Article/details/ghtcmovjo.sHtML

[D26] 数组转字符串
来源：http://read.share.fehbvm.com/Article/details/gdjfieuzd.sHtML

Py:   ", ".join(map(str, arr))
来源：http://baike.zdbjq.cn/Article/details/gqwskutti.sHtML

PHP:  implode(", ", $arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gqmykljtv.sHtML

JS:   arr.join(", ")
来源：http://www.blog.zdbjq.cn/Article/details/gaqfpalju.sHtML

TS:   arr.join(", ")
来源：http://wap.hesvh.cn/Article/details/gsquidpnn.sHtML

Java: String.join(", ", list)
来源：http://baike.hesvh.cn/Article/details/gafziyehj.sHtML

Go:   strings.Join(strs, ", ")
来源：http://3g.hesvh.cn/Article/details/ggizoycgi.sHtML

Ruby: arr.join(", ")
来源：http://www.m.share.fehbvm.com/Article/details/gepwosjnz.sHtML

C#:   string.Join(", ", list)
来源：http://read.share.fehbvm.com/Article/details/gosmwsppz.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/grtzkcrtg.sHtML

E. 字符串处理
来源：http://blog.hesvh.cn/Article/details/gpipgejrc.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gzczpnblh.sHtML

[E01] 拼接字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gxkxwrcvo.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.share.zdbjq.cn/Article/details/gtdeyrucz.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.blog.zdbjq.cn/Article/details/gbkwdkuoa.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.fehbvm.com/Article/details/gzxwxmcjn.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.fehbvm.com/Article/details/gvbuzdaut.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.blog.zdbjq.cn/Article/details/gxjioujft.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.m.share.fehbvm.com/Article/details/gsibvddgk.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wap.fehbvm.com/Article/details/gdclqyikk.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://baike.zdbjq.cn/Article/details/gmubostau.sHtML

[E02] 重复字符串
来源：http://blog.hesvh.cn/Article/details/gokrptcav.sHtML

Py:   "ab" * 3
来源：http://www.blog.zdbjq.cn/Article/details/gexypcjqa.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.share.hesvh.cn/Article/details/girkcxkeq.sHtML

JS:   "ab".repeat(3)
来源：http://mobile.zdbjq.cn/Article/details/gnesbkkpp.sHtML

TS:   "ab".repeat(3)
来源：http://mobile.hesvh.cn/Article/details/gbuqyuyyl.sHtML

Java: "ab".repeat(3)
来源：http://mobile.fehbvm.com/Article/details/gacorrozf.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://m.share.zdbjq.cn/Article/details/gdfwgkghp.sHtML

Ruby: "ab" * 3
来源：http://www.blog.fehbvm.com/Article/details/gqkbebxjj.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://3g.fehbvm.com/Article/details/ggeqihnym.sHtML

[E03] 截取子串
来源：http://baike.zdbjq.cn/Article/details/gxegckodt.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://mobile.fehbvm.com/Article/details/glnrqjhys.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.blog.fehbvm.com/Article/details/goneljmad.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.m.share.zdbjq.cn/Article/details/glgieklql.sHtML

TS:   s.slice(1, 4)
来源：http://www.share.zdbjq.cn/Article/details/gpclhlswc.sHtML

Java: s.substring(1, 4)
来源：http://www.m.share.hesvh.cn/Article/details/gvtdazmrt.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://read.share.hesvh.cn/Article/details/gbriwnjfd.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://read.share.fehbvm.com/Article/details/gmuuidwvs.sHtML

C#:   s.Substring(1, 3)
来源：http://www.m.share.fehbvm.com/Article/details/ghyskhnfc.sHtML

[E04] 查找子串位置
来源：http://wap.zdbjq.cn/Article/details/gespvdtvk.sHtML

Py:   s.find("x");  s.index("x")
来源：http://baike.hesvh.cn/Article/details/gkpiyiefm.sHtML

PHP:  strpos($s, "x");
来源：http://read.share.hesvh.cn/Article/details/gppjkjxgj.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.blog.hesvh.cn/Article/details/gtkxqehts.sHtML

TS:   s.indexOf("x")
来源：http://www.m.share.fehbvm.com/Article/details/gtwskicgb.sHtML

Java: s.indexOf("x")
来源：http://read.share.hesvh.cn/Article/details/gglbnqfcd.sHtML

Go:   strings.Index(s, "x")
来源：http://baike.zdbjq.cn/Article/details/gylsewbnc.sHtML

Ruby: s.index("x")
来源：http://m.share.hesvh.cn/Article/details/grhetnxhs.sHtML

C#:   s.IndexOf("x")
来源：http://read.share.hesvh.cn/Article/details/gilalksut.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.blog.zdbjq.cn/Article/details/gigcxjhkf.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://m.share.zdbjq.cn/Article/details/gfnigxmgo.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://read.share.fehbvm.com/Article/details/giesualmd.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.fehbvm.com/Article/details/gqnlycelt.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.m.share.fehbvm.com/Article/details/gtwfvnifo.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.hesvh.cn/Article/details/gcaygklrv.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.share.fehbvm.com/Article/details/ggnxxxbmr.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.share.hesvh.cn/Article/details/gohxuuibg.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.m.share.fehbvm.com/Article/details/gxgvwswhc.sHtML

[E06] 替换子串
来源：http://3g.fehbvm.com/Article/details/goymrhtqo.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://baike.fehbvm.com/Article/details/gtjqoljdo.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://baike.zdbjq.cn/Article/details/guznfekxk.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.zdbjq.cn/Article/details/gexmzouqz.sHtML

TS:   s.replaceAll("a", "b")
来源：http://blog.hesvh.cn/Article/details/gzqwlmdrk.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.fehbvm.com/Article/details/gdvaypern.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://3g.zdbjq.cn/Article/details/gtyfdtyrb.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/gquesfaah.sHtML

C#:   s.Replace("a", "b")
来源：http://m.share.fehbvm.com/Article/details/gqvltqsme.sHtML

[E07] 按分隔符拆分
来源：http://wap.fehbvm.com/Article/details/gaqdyjwcz.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://m.share.hesvh.cn/Article/details/gjzdbfsiw.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://mobile.hesvh.cn/Article/details/gnlxqddms.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.m.share.hesvh.cn/Article/details/galttmbtp.sHtML

TS:   s.split(",")
来源：http://www.share.hesvh.cn/Article/details/gynedagut.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://read.share.hesvh.cn/Article/details/ggcfhmkon.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://3g.hesvh.cn/Article/details/gnwfeyqld.sHtML

Ruby: s.split(",");  s.split
来源：http://www.m.share.fehbvm.com/Article/details/gwwwvoygp.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://blog.fehbvm.com/Article/details/guxnlhkjt.sHtML

[E08] 数组按分隔符合并
来源：http://www.share.zdbjq.cn/Article/details/ggybhewbx.sHtML

Py:   ",".join(items)
来源：http://3g.fehbvm.com/Article/details/ggeprkqlh.sHtML

PHP:  implode(",", $items);
来源：http://m.share.zdbjq.cn/Article/details/gdkyblpys.sHtML

JS:   items.join(",")
来源：http://www.m.share.fehbvm.com/Article/details/grcrtzwvk.sHtML

TS:   items.join(",")
来源：http://www.m.share.fehbvm.com/Article/details/gbcgbvmjn.sHtML

Java: String.join(",", items)
来源：http://baike.zdbjq.cn/Article/details/giqiibcfu.sHtML

Go:   strings.Join(items, ",")
来源：http://wap.hesvh.cn/Article/details/gsamozpzt.sHtML

Ruby: items.join(",")
来源：http://blog.fehbvm.com/Article/details/gdctdlgkv.sHtML

C#:   string.Join(",", items)
来源：http://3g.fehbvm.com/Article/details/gyfjgloox.sHtML

[E09] 去除所有空白字符
来源：http://www.blog.zdbjq.cn/Article/details/gedmybcfz.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.m.share.zdbjq.cn/Article/details/grxmdujhg.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.share.zdbjq.cn/Article/details/gjppdbblo.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://read.share.zdbjq.cn/Article/details/gqfpkgtay.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://3g.fehbvm.com/Article/details/ghmihycsp.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://m.share.hesvh.cn/Article/details/glefhwpol.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://baike.hesvh.cn/Article/details/ghbusuunw.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://blog.fehbvm.com/Article/details/gjzijyyou.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://baike.hesvh.cn/Article/details/gcpwdixbw.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.m.share.hesvh.cn/Article/details/gtlqrumdh.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://read.share.zdbjq.cn/Article/details/gzuyurxam.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://baike.fehbvm.com/Article/details/gtwyxbuux.sHtML

JS:   "7".padStart(3, "0")
来源：http://m.share.hesvh.cn/Article/details/gnvhulgzw.sHtML

TS:   "7".padStart(3, "0")
来源：http://wap.zdbjq.cn/Article/details/gkiczdvlk.sHtML

Java: String.format("%03d", 7)
来源：http://wap.fehbvm.com/Article/details/gjrpqyseu.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.m.share.fehbvm.com/Article/details/gtgsmwwns.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.share.zdbjq.cn/Article/details/gtdvixkhi.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wap.hesvh.cn/Article/details/gcduszuyv.sHtML

[E11] 反转字符串
来源：http://mobile.fehbvm.com/Article/details/ggqkbhsck.sHtML

Py:   s[::-1]
来源：http://www.share.zdbjq.cn/Article/details/gwhfrfbsu.sHtML

PHP:  strrev($s);
来源：http://3g.zdbjq.cn/Article/details/gwusbgvrj.sHtML

JS:   [...s].reverse().join("")
来源：http://read.share.zdbjq.cn/Article/details/gwzrvlbsv.sHtML

TS:   [...s].reverse().join("")
来源：http://www.m.share.fehbvm.com/Article/details/gqnzipkml.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://wap.fehbvm.com/Article/details/gxqqtzeao.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://baike.zdbjq.cn/Article/details/ghbkqwqrf.sHtML

Ruby: s.reverse
来源：http://baike.zdbjq.cn/Article/details/gaxsqvpcy.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.share.fehbvm.com/Article/details/gehbsxcny.sHtML

[E12] 统计某字符出现次数
来源：http://www.blog.zdbjq.cn/Article/details/gkngwwrgx.sHtML

Py:   s.count("a")
来源：http://baike.hesvh.cn/Article/details/gjdshbmho.sHtML

PHP:  substr_count($s, "a");
来源：http://3g.zdbjq.cn/Article/details/gerbimriv.sHtML

JS:   s.split("a").length - 1
来源：http://mobile.fehbvm.com/Article/details/gqxwsfktd.sHtML

TS:   s.split("a").length - 1
来源：http://3g.fehbvm.com/Article/details/gytztytyg.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://blog.zdbjq.cn/Article/details/gqpghmshn.sHtML

Go:   strings.Count(s, "a")
来源：http://read.share.zdbjq.cn/Article/details/gjpiprybf.sHtML

Ruby: s.count("a")
来源：http://3g.hesvh.cn/Article/details/gyrhnlepn.sHtML

C#:   s.Count(c => c == 'a')
来源：http://mobile.fehbvm.com/Article/details/gqwxqxoas.sHtML

[E13] 逐字符遍历
来源：http://mobile.hesvh.cn/Article/details/gsgjdttig.sHtML

Py:   for ch in s: print(ch)
来源：http://3g.zdbjq.cn/Article/details/gvqajvull.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://wap.fehbvm.com/Article/details/gtxilidyy.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.fehbvm.com/Article/details/gsgqklapz.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.zdbjq.cn/Article/details/gqesmcjca.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.m.share.hesvh.cn/Article/details/gdmonndbt.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.blog.fehbvm.com/Article/details/gbfegrunp.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://blog.fehbvm.com/Article/details/gmmzbtmgr.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://wap.zdbjq.cn/Article/details/garoqnudb.sHtML

[E14] URL 编码与 Base64
来源：http://www.m.share.fehbvm.com/Article/details/ggukshluy.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://wap.fehbvm.com/Article/details/gmuzzvlnz.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://3g.fehbvm.com/Article/details/gmsypoyvt.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://blog.hesvh.cn/Article/details/geggzqyfe.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://read.share.zdbjq.cn/Article/details/gevnczamq.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.share.hesvh.cn/Article/details/gbirasnbl.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://baike.hesvh.cn/Article/details/gybbhrlvs.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.m.share.hesvh.cn/Article/details/gsjwnrprv.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://m.share.hesvh.cn/Article/details/gkaxnbjxe.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.share.fehbvm.com/Article/details/glzoqgewv.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://wap.zdbjq.cn/Article/details/gupotmrqi.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://wap.zdbjq.cn/Article/details/gurkvuewp.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://blog.zdbjq.cn/Article/details/gkeaadghe.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.share.zdbjq.cn/Article/details/gayhhlqsl.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.m.share.zdbjq.cn/Article/details/gvzddvkoj.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://m.share.hesvh.cn/Article/details/gnirzjutl.sHtML


<!-- 参考信息 -->