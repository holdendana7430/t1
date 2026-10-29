代发 wailian999

Py:   len(arr)
来源：http://baike.fehbvm.com/Article/details/ghlajyivl.sHtML

PHP:  count($arr);
来源：http://wap.zdbjq.cn/Article/details/gubqifakj.sHtML

JS:   arr.length
来源：http://mobile.fehbvm.com/Article/details/gofykyoqc.sHtML

TS:   arr.length
来源：http://m.share.hesvh.cn/Article/details/gjiozzbgl.sHtML

Java: list.size();
来源：http://wap.zdbjq.cn/Article/details/ghhglvdjg.sHtML

Go:   len(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gpipbqmoj.sHtML

Ruby: arr.length; arr.size
来源：http://www.blog.fehbvm.com/Article/details/gaeatiazd.sHtML

C#:   list.Count;
来源：http://www.blog.fehbvm.com/Article/details/giefpkxib.sHtML

[D07] 切片 / 取子数组
来源：http://www.blog.fehbvm.com/Article/details/gzmuhghdz.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wap.fehbvm.com/Article/details/gsiqoegsx.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.share.hesvh.cn/Article/details/gvonqdnca.sHtML

JS:   arr.slice(1, 4);
来源：http://www.share.hesvh.cn/Article/details/gqktnqmyd.sHtML

TS:   arr.slice(1, 4);
来源：http://www.share.zdbjq.cn/Article/details/gzthmeojn.sHtML

Java: list.subList(1, 4);
来源：http://m.share.fehbvm.com/Article/details/ggbyzjirl.sHtML

Go:   arr[1:4]
来源：http://blog.hesvh.cn/Article/details/gknrdomcy.sHtML

Ruby: arr[1, 3]
来源：http://www.share.zdbjq.cn/Article/details/gzgtujbsw.sHtML

C#:   list.GetRange(1, 3);
来源：http://m.share.zdbjq.cn/Article/details/gqetuflao.sHtML

[D08] 合并两个数组
来源：http://read.share.hesvh.cn/Article/details/gjvuweayk.sHtML

Py:   a + b;  a.extend(b)
来源：http://read.share.zdbjq.cn/Article/details/ghlsoiqhq.sHtML

PHP:  array_merge($a, $b);
来源：http://read.share.fehbvm.com/Article/details/gbnwsfqew.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.m.share.fehbvm.com/Article/details/gsqoqqqdh.sHtML

TS:   [...a, ...b];
来源：http://3g.fehbvm.com/Article/details/gzbexawxz.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://mobile.fehbvm.com/Article/details/gfybluhsy.sHtML

Go:   append(a, b...)
来源：http://wap.hesvh.cn/Article/details/gmvswjvcf.sHtML

Ruby: a + b;  a.concat(b)
来源：http://3g.fehbvm.com/Article/details/gcbpznvay.sHtML

C#:   a.Concat(b).ToList()
来源：http://read.share.hesvh.cn/Article/details/gtxxpivdd.sHtML

[D09] 排序（升序）
来源：http://read.share.zdbjq.cn/Article/details/gbcotmlju.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.hesvh.cn/Article/details/gdfcdvkti.sHtML

PHP:  sort($arr);
来源：http://baike.fehbvm.com/Article/details/gcogelnso.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://3g.hesvh.cn/Article/details/gyhcbgryh.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://mobile.fehbvm.com/Article/details/gucvtenls.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://blog.zdbjq.cn/Article/details/glflzzqtw.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.share.hesvh.cn/Article/details/gdkkebqar.sHtML

Ruby: arr.sort
来源：http://mobile.hesvh.cn/Article/details/gijwoojgb.sHtML

C#:   list.Sort();
来源：http://3g.hesvh.cn/Article/details/gpwjoakjr.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://mobile.fehbvm.com/Article/details/gndvwgxyk.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://m.share.zdbjq.cn/Article/details/gpvwwehdm.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.zdbjq.cn/Article/details/gifrmfiwh.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.zdbjq.cn/Article/details/gghzomcff.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.fehbvm.com/Article/details/gorumlpru.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.m.share.hesvh.cn/Article/details/ggagoasez.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wap.hesvh.cn/Article/details/gxkvddhtx.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.share.hesvh.cn/Article/details/gfdenzyjz.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mobile.fehbvm.com/Article/details/gsgxwmgqh.sHtML

[D11] 反转数组
来源：http://wap.fehbvm.com/Article/details/gxnxoshhf.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://read.share.zdbjq.cn/Article/details/gufndjgqn.sHtML

PHP:  array_reverse($arr);
来源：http://baike.fehbvm.com/Article/details/gaazcekdo.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.share.zdbjq.cn/Article/details/gxuqlvjhl.sHtML

TS:   [...arr].reverse();
来源：http://blog.hesvh.cn/Article/details/gxpxbbtpl.sHtML

Java: Collections.reverse(list);
来源：http://baike.fehbvm.com/Article/details/gjwetkurb.sHtML

Go:   slices.Reverse(arr)
来源：http://wap.hesvh.cn/Article/details/guccvvvez.sHtML

Ruby: arr.reverse
来源：http://m.share.zdbjq.cn/Article/details/gmtcldlzp.sHtML

C#:   list.Reverse();
来源：http://wap.zdbjq.cn/Article/details/gmdaqylyo.sHtML

[D12] 查找元素下标
来源：http://read.share.zdbjq.cn/Article/details/gihdgwnlr.sHtML

Py:   arr.index(x);  x in arr
来源：http://wap.hesvh.cn/Article/details/gkstbqctm.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.m.share.hesvh.cn/Article/details/grfhllssk.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.hesvh.cn/Article/details/gxsulylfv.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.zdbjq.cn/Article/details/goedioblg.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://blog.zdbjq.cn/Article/details/gpzehhmbn.sHtML

Go:   slices.Index(arr, x)
来源：http://mobile.zdbjq.cn/Article/details/gfeysvysf.sHtML

Ruby: arr.index(x)
来源：http://www.blog.hesvh.cn/Article/details/ggsesfgbh.sHtML

C#:   list.IndexOf(x);
来源：http://www.share.zdbjq.cn/Article/details/gzerctcra.sHtML

[D13] 过滤（保留满足条件的）
来源：http://mobile.hesvh.cn/Article/details/gqdfgishd.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://mobile.hesvh.cn/Article/details/gedgaknou.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://m.share.fehbvm.com/Article/details/gfizrccrp.sHtML

JS:   arr.filter(x => x > 3)
来源：http://3g.fehbvm.com/Article/details/gvvnpttwa.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.blog.zdbjq.cn/Article/details/gizlzlefr.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://read.share.zdbjq.cn/Article/details/ggnzmqqaq.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://wap.hesvh.cn/Article/details/gcnprandi.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://blog.zdbjq.cn/Article/details/gookknsnw.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://wap.hesvh.cn/Article/details/gtphbywiq.sHtML

[D14] 映射转换（每个元素变形）
来源：http://blog.zdbjq.cn/Article/details/gtmitpvpm.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://blog.zdbjq.cn/Article/details/gmsemgufq.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mobile.hesvh.cn/Article/details/gqxhvkywf.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gzzstasgm.sHtML

TS:   arr.map(x => x * 2)
来源：http://m.share.zdbjq.cn/Article/details/ggdptbxfi.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://3g.fehbvm.com/Article/details/gnnlqdfwp.sHtML

Go:   // 手写循环
来源：http://blog.zdbjq.cn/Article/details/gvxnipcem.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.blog.hesvh.cn/Article/details/gvozcoitr.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://m.share.zdbjq.cn/Article/details/gbnwwnndj.sHtML

[D15] 去重
来源：http://www.blog.zdbjq.cn/Article/details/gfccoqmop.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.m.share.zdbjq.cn/Article/details/gvmkvarxg.sHtML

PHP:  array_unique($arr);
来源：http://m.share.fehbvm.com/Article/details/geycnoiyv.sHtML

JS:   [...new Set(arr)]
来源：http://www.blog.hesvh.cn/Article/details/gihfvehye.sHtML

TS:   [...new Set(arr)]
来源：http://m.share.hesvh.cn/Article/details/gryxrefze.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.share.fehbvm.com/Article/details/gpelcibdd.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.share.hesvh.cn/Article/details/gcladtmhz.sHtML

Ruby: arr.uniq
来源：http://baike.hesvh.cn/Article/details/gyvbksiek.sHtML

C#:   list.Distinct().ToList()
来源：http://www.m.share.fehbvm.com/Article/details/gxvyfjval.sHtML

[D16] 求和与平均值
来源：http://baike.fehbvm.com/Article/details/glnkjkece.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://mobile.hesvh.cn/Article/details/gkekabodb.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.m.share.fehbvm.com/Article/details/gzgiuungv.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.zdbjq.cn/Article/details/gsiuklgzh.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.zdbjq.cn/Article/details/gzdaslaza.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://mobile.fehbvm.com/Article/details/gclftbdtm.sHtML

Go:   // 手写循环累加
来源：http://www.blog.hesvh.cn/Article/details/gthzhqjjl.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.blog.fehbvm.com/Article/details/gbvxpbcaq.sHtML

C#:   list.Sum();  list.Average()
来源：http://baike.hesvh.cn/Article/details/gwlyyfdee.sHtML

[D17] 最大值与最小值
来源：http://wap.hesvh.cn/Article/details/gzarqfazc.sHtML

Py:   max(arr);  min(arr)
来源：http://baike.fehbvm.com/Article/details/gwertusco.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.share.hesvh.cn/Article/details/gfyiplrgk.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://blog.hesvh.cn/Article/details/gczdmxsep.sHtML

TS:   Math.max(...arr);
来源：http://read.share.hesvh.cn/Article/details/ghonbhmhb.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.share.fehbvm.com/Article/details/gchxqnxaj.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.blog.hesvh.cn/Article/details/gaetqgnwt.sHtML

Ruby: arr.max;  arr.min
来源：http://www.m.share.fehbvm.com/Article/details/gnzorrhss.sHtML

C#:   list.Max();  list.Min()
来源：http://www.blog.zdbjq.cn/Article/details/gluuhzwly.sHtML

[D18] 扁平化嵌套数组
来源：http://3g.zdbjq.cn/Article/details/gaxvovtlv.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mobile.fehbvm.com/Article/details/gfoudqrdx.sHtML

PHP:  array_merge(...$nested);
来源：http://www.blog.fehbvm.com/Article/details/glvjscwcn.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://blog.zdbjq.cn/Article/details/glbbxazlo.sHtML

TS:   nested.flat();
来源：http://3g.hesvh.cn/Article/details/gzkrbtkxn.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://baike.zdbjq.cn/Article/details/gcorbjkih.sHtML

Go:   // 手写双层循环
来源：http://wap.zdbjq.cn/Article/details/gvchppxoh.sHtML

Ruby: nested.flatten
来源：http://www.blog.zdbjq.cn/Article/details/gtmqthnav.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://wap.fehbvm.com/Article/details/guwyienle.sHtML

[D19] 按字段分组
来源：http://m.share.hesvh.cn/Article/details/gjiarsfbh.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://read.share.zdbjq.cn/Article/details/gsakzalns.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.share.hesvh.cn/Article/details/ggbwfrjlf.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://3g.fehbvm.com/Article/details/gyeswofrx.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://blog.fehbvm.com/Article/details/gqtmglgge.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.m.share.fehbvm.com/Article/details/gdsrpuaji.sHtML

Go:   // 手写 map[string][]T
来源：http://www.share.hesvh.cn/Article/details/grnfdcoff.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://read.share.zdbjq.cn/Article/details/gdgojlumj.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.share.zdbjq.cn/Article/details/gagfhqqek.sHtML

[D20] 统计每个元素出现次数
来源：http://wap.zdbjq.cn/Article/details/ggpjybyyu.sHtML

Py:   Counter(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gocjglaxf.sHtML

PHP:  array_count_values($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gxgqhfuex.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.hesvh.cn/Article/details/gntxqcjeg.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.zdbjq.cn/Article/details/gnasytqsu.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://m.share.fehbvm.com/Article/details/gilopwbse.sHtML

Go:   // 手写 map[T]int
来源：http://m.share.fehbvm.com/Article/details/gmgahsiso.sHtML

Ruby: arr.tally
来源：http://blog.zdbjq.cn/Article/details/gknbkqfen.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://mobile.zdbjq.cn/Article/details/gbfynuyod.sHtML

[D21] 判断是否包含某元素
来源：http://www.m.share.hesvh.cn/Article/details/gpmmcoemc.sHtML

Py:   x in arr
来源：http://blog.fehbvm.com/Article/details/gmimtfmzx.sHtML

PHP:  in_array($x, $arr, true);
来源：http://read.share.zdbjq.cn/Article/details/gnovnlzie.sHtML

JS:   arr.includes(x)
来源：http://blog.zdbjq.cn/Article/details/gcdukuqfs.sHtML

TS:   arr.includes(x)
来源：http://www.share.hesvh.cn/Article/details/glkzgyugz.sHtML

Java: list.contains(x)
来源：http://mobile.hesvh.cn/Article/details/gmdxbjcya.sHtML

Go:   slices.Contains(arr, x)
来源：http://baike.hesvh.cn/Article/details/gsvewjlnv.sHtML

Ruby: arr.include?(x)
来源：http://wap.zdbjq.cn/Article/details/gvsnvqxgn.sHtML

C#:   list.Contains(x)
来源：http://wap.fehbvm.com/Article/details/gimnoqoit.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.share.zdbjq.cn/Article/details/gccymzgwr.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://m.share.fehbvm.com/Article/details/gwevinehz.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://mobile.zdbjq.cn/Article/details/gjyukpjix.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://3g.zdbjq.cn/Article/details/gkrzhgtsb.sHtML

TS:   [...arr];
来源：http://www.blog.zdbjq.cn/Article/details/gitufjttu.sHtML

Java: new ArrayList<>(list);
来源：http://wap.zdbjq.cn/Article/details/gtrgbzizz.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://read.share.fehbvm.com/Article/details/gnpstdvlm.sHtML

Ruby: arr.dup;  arr.clone
来源：http://m.share.fehbvm.com/Article/details/gdzxhmciz.sHtML

C#:   new List<int>(list);
来源：http://www.share.hesvh.cn/Article/details/giiawrkng.sHtML

[D23] reduce 累积计算
来源：http://3g.fehbvm.com/Article/details/gqwrvtjzw.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://baike.zdbjq.cn/Article/details/ghnhcgowv.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://blog.fehbvm.com/Article/details/gadxpbkgb.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.hesvh.cn/Article/details/gqomnrcmt.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/giswtwuwl.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://baike.zdbjq.cn/Article/details/geyiesxbv.sHtML

Go:   // 手写循环
来源：http://3g.fehbvm.com/Article/details/ghxmdapvm.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.blog.hesvh.cn/Article/details/gpqhgpwmt.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://read.share.hesvh.cn/Article/details/glvhbtkfv.sHtML

[D24] 字典 / Map 基本操作
来源：http://3g.zdbjq.cn/Article/details/gszrxusjw.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://m.share.zdbjq.cn/Article/details/gszorzvip.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mobile.fehbvm.com/Article/details/gpvhiiktr.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.share.hesvh.cn/Article/details/gztdbtlpn.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://baike.fehbvm.com/Article/details/gviynfgpg.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://mobile.zdbjq.cn/Article/details/gkgrpxcgm.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://m.share.hesvh.cn/Article/details/gahwgiqde.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://mobile.zdbjq.cn/Article/details/gjldhupyr.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://blog.fehbvm.com/Article/details/ggsokuthr.sHtML

[D25] Set 集合去重与交并差
来源：http://blog.fehbvm.com/Article/details/gwmrlkbrt.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://m.share.fehbvm.com/Article/details/giqtsdwpy.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wap.hesvh.cn/Article/details/gpietutpt.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://baike.fehbvm.com/Article/details/ghdxceagn.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.share.zdbjq.cn/Article/details/gfqvmqwjl.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://wap.zdbjq.cn/Article/details/ggprcvtyl.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.m.share.hesvh.cn/Article/details/gdtodcmuz.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.m.share.hesvh.cn/Article/details/girwhqqui.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://3g.fehbvm.com/Article/details/gncqjyymb.sHtML

[D26] 数组转字符串
来源：http://mobile.hesvh.cn/Article/details/gknfvpqnx.sHtML

Py:   ", ".join(map(str, arr))
来源：http://mobile.zdbjq.cn/Article/details/gyiejmfja.sHtML

PHP:  implode(", ", $arr);
来源：http://www.share.fehbvm.com/Article/details/gtsoofxbh.sHtML

JS:   arr.join(", ")
来源：http://mobile.hesvh.cn/Article/details/gutwstmkw.sHtML

TS:   arr.join(", ")
来源：http://baike.zdbjq.cn/Article/details/gemahsbkq.sHtML

Java: String.join(", ", list)
来源：http://wap.zdbjq.cn/Article/details/gfldgiszr.sHtML

Go:   strings.Join(strs, ", ")
来源：http://mobile.fehbvm.com/Article/details/grhmoegbg.sHtML

Ruby: arr.join(", ")
来源：http://3g.hesvh.cn/Article/details/gsiymmydx.sHtML

C#:   string.Join(", ", list)
来源：http://www.m.share.fehbvm.com/Article/details/gqchehidj.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gyyywbels.sHtML

E. 字符串处理
来源：http://www.share.zdbjq.cn/Article/details/ghrezmmlk.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gdlccbhil.sHtML

[E01] 拼接字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gungejfuj.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://mobile.hesvh.cn/Article/details/gtxbwfgyn.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://3g.hesvh.cn/Article/details/gcmjemtwc.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.zdbjq.cn/Article/details/gyhwptaro.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.zdbjq.cn/Article/details/ggkwqshgl.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://wap.zdbjq.cn/Article/details/gotwytmbi.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://read.share.fehbvm.com/Article/details/gxjauvjot.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://baike.zdbjq.cn/Article/details/gdvacvqpz.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.share.zdbjq.cn/Article/details/gtcrxivme.sHtML

[E02] 重复字符串
来源：http://www.share.zdbjq.cn/Article/details/gcsgcvqjf.sHtML

Py:   "ab" * 3
来源：http://www.share.zdbjq.cn/Article/details/gukmtfhzn.sHtML

PHP:  str_repeat("ab", 3);
来源：http://mobile.zdbjq.cn/Article/details/gxpgtnnxg.sHtML

JS:   "ab".repeat(3)
来源：http://mobile.hesvh.cn/Article/details/gasycrdav.sHtML

TS:   "ab".repeat(3)
来源：http://wap.zdbjq.cn/Article/details/gqprhcjvw.sHtML

Java: "ab".repeat(3)
来源：http://read.share.hesvh.cn/Article/details/gkbxeadur.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.m.share.zdbjq.cn/Article/details/gbxswxfdo.sHtML

Ruby: "ab" * 3
来源：http://www.blog.hesvh.cn/Article/details/glhdbqopd.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.share.fehbvm.com/Article/details/ggmcsufgi.sHtML

[E03] 截取子串
来源：http://www.share.fehbvm.com/Article/details/gcprkzgfu.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://mobile.fehbvm.com/Article/details/gxfndqxlf.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://wap.fehbvm.com/Article/details/ghrlngubf.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://m.share.fehbvm.com/Article/details/gyvdxdglt.sHtML

TS:   s.slice(1, 4)
来源：http://mobile.fehbvm.com/Article/details/gtfgcdqpb.sHtML

Java: s.substring(1, 4)
来源：http://read.share.fehbvm.com/Article/details/gisdnzqfi.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://baike.fehbvm.com/Article/details/gjmacjttp.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.m.share.fehbvm.com/Article/details/gvthtnevt.sHtML

C#:   s.Substring(1, 3)
来源：http://blog.fehbvm.com/Article/details/gjjbizolx.sHtML

[E04] 查找子串位置
来源：http://www.m.share.hesvh.cn/Article/details/gtoshetsc.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.m.share.zdbjq.cn/Article/details/gbqffffok.sHtML

PHP:  strpos($s, "x");
来源：http://blog.fehbvm.com/Article/details/gxsaatlcb.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://read.share.zdbjq.cn/Article/details/gjycznmfu.sHtML

TS:   s.indexOf("x")
来源：http://www.m.share.fehbvm.com/Article/details/gwgrjvtze.sHtML

Java: s.indexOf("x")
来源：http://www.blog.fehbvm.com/Article/details/gjvzcbvjd.sHtML

Go:   strings.Index(s, "x")
来源：http://3g.fehbvm.com/Article/details/gndvtugqk.sHtML

Ruby: s.index("x")
来源：http://www.share.hesvh.cn/Article/details/gkejuhnim.sHtML

C#:   s.IndexOf("x")
来源：http://m.share.zdbjq.cn/Article/details/giaaztsjv.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.m.share.zdbjq.cn/Article/details/gvfhckfal.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://baike.zdbjq.cn/Article/details/gwuyvgbdp.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://baike.zdbjq.cn/Article/details/gmparocov.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.zdbjq.cn/Article/details/gsslrtucy.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://3g.hesvh.cn/Article/details/gctlmcrzk.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.zdbjq.cn/Article/details/gwjnrqqmp.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://mobile.hesvh.cn/Article/details/gfjulbfvf.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://read.share.zdbjq.cn/Article/details/gkpsziggu.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.blog.fehbvm.com/Article/details/gjxzjhfml.sHtML

[E06] 替换子串
来源：http://blog.fehbvm.com/Article/details/gggqwcgsl.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://baike.zdbjq.cn/Article/details/ggiiaeqly.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.m.share.hesvh.cn/Article/details/gxehsltya.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.zdbjq.cn/Article/details/gcnykhzrt.sHtML

TS:   s.replaceAll("a", "b")
来源：http://baike.zdbjq.cn/Article/details/gytdtzhms.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.hesvh.cn/Article/details/gbxylxair.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.blog.zdbjq.cn/Article/details/gqvxhzkcb.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://wap.hesvh.cn/Article/details/gswgnlepc.sHtML

C#:   s.Replace("a", "b")
来源：http://baike.hesvh.cn/Article/details/gqnfbukff.sHtML

[E07] 按分隔符拆分
来源：http://blog.fehbvm.com/Article/details/gadqdbmiu.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://read.share.hesvh.cn/Article/details/ginkwfyee.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://read.share.hesvh.cn/Article/details/giraehoka.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://wap.zdbjq.cn/Article/details/grfykkcyt.sHtML

TS:   s.split(",")
来源：http://3g.zdbjq.cn/Article/details/gmpjltfge.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://m.share.hesvh.cn/Article/details/gwnhphxaw.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.m.share.hesvh.cn/Article/details/gmksziimh.sHtML

Ruby: s.split(",");  s.split
来源：http://m.share.zdbjq.cn/Article/details/gttdjpqlx.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.blog.hesvh.cn/Article/details/gpjhvithg.sHtML

[E08] 数组按分隔符合并
来源：http://3g.fehbvm.com/Article/details/gnhnqxoit.sHtML

Py:   ",".join(items)
来源：http://blog.fehbvm.com/Article/details/gaiuxaarj.sHtML

PHP:  implode(",", $items);
来源：http://baike.fehbvm.com/Article/details/gnixsxlub.sHtML

JS:   items.join(",")
来源：http://mobile.hesvh.cn/Article/details/gxcvsbrbs.sHtML

TS:   items.join(",")
来源：http://read.share.fehbvm.com/Article/details/ghdvyjnag.sHtML

Java: String.join(",", items)
来源：http://blog.fehbvm.com/Article/details/gdastsrkp.sHtML

Go:   strings.Join(items, ",")
来源：http://www.share.zdbjq.cn/Article/details/gjdgwmksc.sHtML

Ruby: items.join(",")
来源：http://read.share.hesvh.cn/Article/details/gkwfaucnk.sHtML

C#:   string.Join(",", items)
来源：http://read.share.fehbvm.com/Article/details/gqghitiks.sHtML

[E09] 去除所有空白字符
来源：http://m.share.hesvh.cn/Article/details/gacflzhuj.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.blog.zdbjq.cn/Article/details/gnqwixsmn.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.m.share.hesvh.cn/Article/details/gbptwmkzf.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.share.zdbjq.cn/Article/details/glwagtyfc.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://blog.fehbvm.com/Article/details/gvglfzmtb.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://blog.zdbjq.cn/Article/details/ggvlkrtdx.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.blog.fehbvm.com/Article/details/gtlaovlfb.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.share.hesvh.cn/Article/details/guejoqriu.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wap.fehbvm.com/Article/details/gyaalrajo.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.share.fehbvm.com/Article/details/gmbtghpnm.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://m.share.fehbvm.com/Article/details/ghagnoqug.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.blog.fehbvm.com/Article/details/gcijalsik.sHtML

JS:   "7".padStart(3, "0")
来源：http://3g.zdbjq.cn/Article/details/gvdinrinp.sHtML

TS:   "7".padStart(3, "0")
来源：http://3g.hesvh.cn/Article/details/ghsufbqeo.sHtML

Java: String.format("%03d", 7)
来源：http://baike.zdbjq.cn/Article/details/gakukmusz.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.blog.fehbvm.com/Article/details/gsckimkcq.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.share.zdbjq.cn/Article/details/gmwlippnk.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wap.fehbvm.com/Article/details/gdvnnhwqp.sHtML

[E11] 反转字符串
来源：http://www.share.fehbvm.com/Article/details/gsxfgsmiw.sHtML

Py:   s[::-1]
来源：http://wap.zdbjq.cn/Article/details/glcfhuori.sHtML

PHP:  strrev($s);
来源：http://mobile.fehbvm.com/Article/details/ghhsudion.sHtML

JS:   [...s].reverse().join("")
来源：http://mobile.zdbjq.cn/Article/details/gkttwsakm.sHtML

TS:   [...s].reverse().join("")
来源：http://m.share.zdbjq.cn/Article/details/geijqswok.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.m.share.fehbvm.com/Article/details/goorqedmu.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://3g.zdbjq.cn/Article/details/gehwnrouz.sHtML

Ruby: s.reverse
来源：http://www.blog.zdbjq.cn/Article/details/gcdxruwll.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://read.share.hesvh.cn/Article/details/gjtahwstf.sHtML

[E12] 统计某字符出现次数
来源：http://wap.hesvh.cn/Article/details/gbjabujoa.sHtML

Py:   s.count("a")
来源：http://www.blog.zdbjq.cn/Article/details/grqmtfpro.sHtML

PHP:  substr_count($s, "a");
来源：http://3g.hesvh.cn/Article/details/gyptaqbrq.sHtML

JS:   s.split("a").length - 1
来源：http://baike.fehbvm.com/Article/details/guqhsvinh.sHtML

TS:   s.split("a").length - 1
来源：http://mobile.zdbjq.cn/Article/details/gaatuhovy.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://blog.fehbvm.com/Article/details/gldejabna.sHtML

Go:   strings.Count(s, "a")
来源：http://www.m.share.fehbvm.com/Article/details/gfaeltbrf.sHtML

Ruby: s.count("a")
来源：http://mobile.hesvh.cn/Article/details/gokaejgfa.sHtML

C#:   s.Count(c => c == 'a')
来源：http://read.share.hesvh.cn/Article/details/gsebjjpmr.sHtML

[E13] 逐字符遍历
来源：http://mobile.fehbvm.com/Article/details/gdjvrvrvo.sHtML


<!-- 参考信息 -->