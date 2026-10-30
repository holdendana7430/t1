代发 wailian999

Go:   arr[0]; arr[0] = 9
来源：http://read.share.fehbvm.com/Article/details/giviazutu.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.hesvh.cn/Article/details/gvorcnmxt.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://blog.fehbvm.com/Article/details/ggqroekxy.sHtML

[D06] 数组长度
来源：http://www.blog.zdbjq.cn/Article/details/gngjlplwd.sHtML

Py:   len(arr)
来源：http://wap.hesvh.cn/Article/details/gvvrtgwzc.sHtML

PHP:  count($arr);
来源：http://m.share.hesvh.cn/Article/details/gcgzcwqyo.sHtML

JS:   arr.length
来源：http://www.blog.zdbjq.cn/Article/details/gpccbnaiw.sHtML

TS:   arr.length
来源：http://wap.zdbjq.cn/Article/details/gyyrivcvd.sHtML

Java: list.size();
来源：http://blog.fehbvm.com/Article/details/gkwjgazff.sHtML

Go:   len(arr)
来源：http://mobile.zdbjq.cn/Article/details/gcyxfevre.sHtML

Ruby: arr.length; arr.size
来源：http://www.share.zdbjq.cn/Article/details/geangsvin.sHtML

C#:   list.Count;
来源：http://baike.hesvh.cn/Article/details/gqpubeqgp.sHtML

[D07] 切片 / 取子数组
来源：http://www.m.share.zdbjq.cn/Article/details/gclfbfcyb.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wap.hesvh.cn/Article/details/gwtaudsek.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.m.share.fehbvm.com/Article/details/gmhydbcsi.sHtML

JS:   arr.slice(1, 4);
来源：http://read.share.fehbvm.com/Article/details/gorjgkfmd.sHtML

TS:   arr.slice(1, 4);
来源：http://www.blog.zdbjq.cn/Article/details/gvjzokqgj.sHtML

Java: list.subList(1, 4);
来源：http://www.share.zdbjq.cn/Article/details/gsoqtnynw.sHtML

Go:   arr[1:4]
来源：http://mobile.zdbjq.cn/Article/details/gsjjjemak.sHtML

Ruby: arr[1, 3]
来源：http://www.share.hesvh.cn/Article/details/ghszxawfu.sHtML

C#:   list.GetRange(1, 3);
来源：http://baike.zdbjq.cn/Article/details/gkjdfvvjh.sHtML

[D08] 合并两个数组
来源：http://m.share.hesvh.cn/Article/details/ggeebllms.sHtML

Py:   a + b;  a.extend(b)
来源：http://read.share.zdbjq.cn/Article/details/gpvptdhyu.sHtML

PHP:  array_merge($a, $b);
来源：http://www.share.hesvh.cn/Article/details/gsphhmvfd.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.share.zdbjq.cn/Article/details/gerbeices.sHtML

TS:   [...a, ...b];
来源：http://baike.fehbvm.com/Article/details/gknwpgldv.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://read.share.fehbvm.com/Article/details/gdjxagxyp.sHtML

Go:   append(a, b...)
来源：http://blog.fehbvm.com/Article/details/glrpwilmu.sHtML

Ruby: a + b;  a.concat(b)
来源：http://baike.fehbvm.com/Article/details/gixzovkyx.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.share.fehbvm.com/Article/details/gwyvpwozn.sHtML

[D09] 排序（升序）
来源：http://read.share.fehbvm.com/Article/details/gmpgbfgzo.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.zdbjq.cn/Article/details/gbrmsvzsi.sHtML

PHP:  sort($arr);
来源：http://read.share.fehbvm.com/Article/details/gvswftjbl.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.blog.hesvh.cn/Article/details/gvoqpjwak.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://blog.fehbvm.com/Article/details/geqnxiien.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://m.share.fehbvm.com/Article/details/gudcvwkre.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.m.share.fehbvm.com/Article/details/giyizigjp.sHtML

Ruby: arr.sort
来源：http://m.share.fehbvm.com/Article/details/gyuxuwexn.sHtML

C#:   list.Sort();
来源：http://wap.hesvh.cn/Article/details/gbzwkhhaf.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://3g.zdbjq.cn/Article/details/gaoepcgci.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.blog.fehbvm.com/Article/details/gvrqqaggb.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.fehbvm.com/Article/details/gkbugygrx.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.fehbvm.com/Article/details/gjihcculq.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.hesvh.cn/Article/details/ggrhrecpe.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.blog.hesvh.cn/Article/details/gqvkwirdn.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://m.share.fehbvm.com/Article/details/grabxuyzu.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mobile.fehbvm.com/Article/details/gnagtstqj.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://3g.fehbvm.com/Article/details/gooskmqte.sHtML

[D11] 反转数组
来源：http://3g.hesvh.cn/Article/details/gkjknogvb.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.share.hesvh.cn/Article/details/gydrsnsih.sHtML

PHP:  array_reverse($arr);
来源：http://3g.fehbvm.com/Article/details/gwxshedxn.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.blog.fehbvm.com/Article/details/gsvsxjcnc.sHtML

TS:   [...arr].reverse();
来源：http://blog.zdbjq.cn/Article/details/gytewziup.sHtML

Java: Collections.reverse(list);
来源：http://www.share.zdbjq.cn/Article/details/gnqigvoqk.sHtML

Go:   slices.Reverse(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/grfgauijl.sHtML

Ruby: arr.reverse
来源：http://read.share.hesvh.cn/Article/details/gluntuicd.sHtML

C#:   list.Reverse();
来源：http://baike.zdbjq.cn/Article/details/gqiedvvxe.sHtML

[D12] 查找元素下标
来源：http://www.blog.fehbvm.com/Article/details/gfcrhsbgc.sHtML

Py:   arr.index(x);  x in arr
来源：http://baike.hesvh.cn/Article/details/gnwshtxcc.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://baike.zdbjq.cn/Article/details/gkitqypxg.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.zdbjq.cn/Article/details/gwamyjkdc.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.hesvh.cn/Article/details/gcxiygzco.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://blog.hesvh.cn/Article/details/gaqacizth.sHtML

Go:   slices.Index(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/ghjsjrumv.sHtML

Ruby: arr.index(x)
来源：http://blog.zdbjq.cn/Article/details/guagmqlhe.sHtML

C#:   list.IndexOf(x);
来源：http://m.share.hesvh.cn/Article/details/gugxhsvch.sHtML

[D13] 过滤（保留满足条件的）
来源：http://blog.hesvh.cn/Article/details/glxsnqmtg.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://wap.zdbjq.cn/Article/details/gztrcbssj.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.m.share.hesvh.cn/Article/details/gkodspluu.sHtML

JS:   arr.filter(x => x > 3)
来源：http://blog.zdbjq.cn/Article/details/gxawjuhkl.sHtML

TS:   arr.filter(x => x > 3)
来源：http://baike.fehbvm.com/Article/details/gcfhjovtz.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://baike.fehbvm.com/Article/details/geyecsnei.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.blog.hesvh.cn/Article/details/gurbqqhxw.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.blog.hesvh.cn/Article/details/gynkzucma.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://baike.hesvh.cn/Article/details/gkubnfskg.sHtML

[D14] 映射转换（每个元素变形）
来源：http://mobile.zdbjq.cn/Article/details/gewlpmkok.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://3g.fehbvm.com/Article/details/gokmlqnuu.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.share.hesvh.cn/Article/details/garolujgp.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.share.hesvh.cn/Article/details/ghgnleuhg.sHtML

TS:   arr.map(x => x * 2)
来源：http://read.share.fehbvm.com/Article/details/glvrijtrf.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://blog.zdbjq.cn/Article/details/gkgqpxaho.sHtML

Go:   // 手写循环
来源：http://www.blog.zdbjq.cn/Article/details/gticansqc.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://m.share.fehbvm.com/Article/details/gotyrailr.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.share.hesvh.cn/Article/details/ggrjymhxu.sHtML

[D15] 去重
来源：http://mobile.fehbvm.com/Article/details/gqlwdgpyc.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://baike.zdbjq.cn/Article/details/gzecitpkf.sHtML

PHP:  array_unique($arr);
来源：http://mobile.fehbvm.com/Article/details/gzmzkfehf.sHtML

JS:   [...new Set(arr)]
来源：http://wap.hesvh.cn/Article/details/gyhpzxsdf.sHtML

TS:   [...new Set(arr)]
来源：http://www.blog.fehbvm.com/Article/details/gutdvlgbm.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://m.share.hesvh.cn/Article/details/gcpqtjzkb.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://read.share.zdbjq.cn/Article/details/gurvbrpou.sHtML

Ruby: arr.uniq
来源：http://m.share.zdbjq.cn/Article/details/grqwkolem.sHtML

C#:   list.Distinct().ToList()
来源：http://baike.zdbjq.cn/Article/details/gaytxbuxe.sHtML

[D16] 求和与平均值
来源：http://wap.fehbvm.com/Article/details/gzqgxwlft.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gogyfyltg.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://3g.zdbjq.cn/Article/details/gdoltjkgm.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.zdbjq.cn/Article/details/gkidkpscb.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.fehbvm.com/Article/details/gdmzkzcbs.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://mobile.zdbjq.cn/Article/details/gvvsmyabm.sHtML

Go:   // 手写循环累加
来源：http://read.share.zdbjq.cn/Article/details/geckviorj.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://blog.zdbjq.cn/Article/details/gafngvsac.sHtML

C#:   list.Sum();  list.Average()
来源：http://blog.hesvh.cn/Article/details/gsntujrsg.sHtML

[D17] 最大值与最小值
来源：http://www.share.hesvh.cn/Article/details/gixczhykf.sHtML

Py:   max(arr);  min(arr)
来源：http://baike.hesvh.cn/Article/details/grmzopnaa.sHtML

PHP:  max($arr);  min($arr);
来源：http://mobile.fehbvm.com/Article/details/gtbbksdbb.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.share.zdbjq.cn/Article/details/gvytbybup.sHtML

TS:   Math.max(...arr);
来源：http://baike.hesvh.cn/Article/details/gfwwpdrhu.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.blog.zdbjq.cn/Article/details/ghfazqzbg.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.share.hesvh.cn/Article/details/gzfspyqjt.sHtML

Ruby: arr.max;  arr.min
来源：http://www.m.share.fehbvm.com/Article/details/gogyuzmpa.sHtML

C#:   list.Max();  list.Min()
来源：http://m.share.zdbjq.cn/Article/details/gqyeprrbj.sHtML

[D18] 扁平化嵌套数组
来源：http://mobile.hesvh.cn/Article/details/gwyhvnqgj.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mobile.hesvh.cn/Article/details/gpuimmoen.sHtML

PHP:  array_merge(...$nested);
来源：http://www.blog.zdbjq.cn/Article/details/gyobhetes.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.m.share.hesvh.cn/Article/details/gimxwxszy.sHtML

TS:   nested.flat();
来源：http://www.m.share.zdbjq.cn/Article/details/gaoqrnwsk.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wap.hesvh.cn/Article/details/gtebgjugb.sHtML

Go:   // 手写双层循环
来源：http://m.share.zdbjq.cn/Article/details/gekipsrse.sHtML

Ruby: nested.flatten
来源：http://wap.hesvh.cn/Article/details/gmwbyedjj.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://3g.hesvh.cn/Article/details/gdntetydv.sHtML

[D19] 按字段分组
来源：http://read.share.fehbvm.com/Article/details/gfkrfdhel.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://3g.fehbvm.com/Article/details/gjtlhvbcs.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.share.zdbjq.cn/Article/details/gkytrkdko.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://blog.fehbvm.com/Article/details/guunzbusf.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://read.share.hesvh.cn/Article/details/gzqomlxvw.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.share.hesvh.cn/Article/details/gofnvsdee.sHtML

Go:   // 手写 map[string][]T
来源：http://www.blog.zdbjq.cn/Article/details/gagyecwux.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://wap.hesvh.cn/Article/details/gnddoqigi.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wap.fehbvm.com/Article/details/guwqphqma.sHtML

[D20] 统计每个元素出现次数
来源：http://baike.zdbjq.cn/Article/details/gduzmythv.sHtML

Py:   Counter(arr)
来源：http://mobile.fehbvm.com/Article/details/ggclclpag.sHtML

PHP:  array_count_values($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/guexxncjo.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.fehbvm.com/Article/details/gruatuoca.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.hesvh.cn/Article/details/ggvbufbls.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wap.hesvh.cn/Article/details/gplasbkwx.sHtML

Go:   // 手写 map[T]int
来源：http://3g.hesvh.cn/Article/details/gohvcenab.sHtML

Ruby: arr.tally
来源：http://wap.fehbvm.com/Article/details/givtpngrg.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://blog.hesvh.cn/Article/details/gjdfdnipu.sHtML

[D21] 判断是否包含某元素
来源：http://mobile.hesvh.cn/Article/details/gbqsaqmjy.sHtML

Py:   x in arr
来源：http://blog.hesvh.cn/Article/details/geeptijap.sHtML

PHP:  in_array($x, $arr, true);
来源：http://baike.zdbjq.cn/Article/details/gruumyzzy.sHtML

JS:   arr.includes(x)
来源：http://mobile.hesvh.cn/Article/details/glwrptzhe.sHtML

TS:   arr.includes(x)
来源：http://baike.zdbjq.cn/Article/details/gejkbzoeq.sHtML

Java: list.contains(x)
来源：http://www.m.share.hesvh.cn/Article/details/gxohdphsa.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.share.hesvh.cn/Article/details/gsxlrfnfi.sHtML

Ruby: arr.include?(x)
来源：http://wap.fehbvm.com/Article/details/gbgggzowu.sHtML

C#:   list.Contains(x)
来源：http://baike.zdbjq.cn/Article/details/gjiifhkbl.sHtML

[D22] 复制数组（避免共享引用）
来源：http://wap.hesvh.cn/Article/details/giwseunww.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://blog.zdbjq.cn/Article/details/ghaeianpu.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://mobile.fehbvm.com/Article/details/gvarackcl.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://3g.hesvh.cn/Article/details/gjrtibhem.sHtML

TS:   [...arr];
来源：http://baike.hesvh.cn/Article/details/gamtcclkc.sHtML

Java: new ArrayList<>(list);
来源：http://wap.fehbvm.com/Article/details/goytxikmz.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://m.share.zdbjq.cn/Article/details/gewwwwslv.sHtML

Ruby: arr.dup;  arr.clone
来源：http://m.share.hesvh.cn/Article/details/geblytunl.sHtML

C#:   new List<int>(list);
来源：http://www.m.share.hesvh.cn/Article/details/gqcpehzny.sHtML

[D23] reduce 累积计算
来源：http://mobile.fehbvm.com/Article/details/goaeotjsn.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://blog.fehbvm.com/Article/details/gzanrgzhq.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://read.share.hesvh.cn/Article/details/ghpvuoypx.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.zdbjq.cn/Article/details/gdltxxawe.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.hesvh.cn/Article/details/gwgqomkbu.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://3g.zdbjq.cn/Article/details/ggitjrpta.sHtML

Go:   // 手写循环
来源：http://www.share.hesvh.cn/Article/details/gotuayqst.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.blog.zdbjq.cn/Article/details/gdmduqjjb.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mobile.fehbvm.com/Article/details/grtnkmrlx.sHtML

[D24] 字典 / Map 基本操作
来源：http://blog.hesvh.cn/Article/details/geklmjxur.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.m.share.zdbjq.cn/Article/details/gxibsenhh.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.blog.zdbjq.cn/Article/details/gadrydsqk.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.blog.hesvh.cn/Article/details/ghyfdwigd.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.blog.hesvh.cn/Article/details/gdgplxbgp.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://mobile.zdbjq.cn/Article/details/gtvbrhwer.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.blog.fehbvm.com/Article/details/gozlxvqei.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://wap.zdbjq.cn/Article/details/gaazkynrh.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wap.fehbvm.com/Article/details/gowzshjsd.sHtML

[D25] Set 集合去重与交并差
来源：http://blog.hesvh.cn/Article/details/gluldvaba.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://blog.zdbjq.cn/Article/details/gcxmeoejz.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.share.zdbjq.cn/Article/details/gwxhjjghi.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://read.share.hesvh.cn/Article/details/gfkvbvtrl.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.share.hesvh.cn/Article/details/gywgvmyuh.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://baike.hesvh.cn/Article/details/glhljduok.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://3g.fehbvm.com/Article/details/gbmfoytlt.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://m.share.hesvh.cn/Article/details/gizfguacl.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.m.share.fehbvm.com/Article/details/gbiiftshq.sHtML

[D26] 数组转字符串
来源：http://baike.zdbjq.cn/Article/details/gbydrmutq.sHtML

Py:   ", ".join(map(str, arr))
来源：http://mobile.fehbvm.com/Article/details/gzhuzrvgl.sHtML

PHP:  implode(", ", $arr);
来源：http://www.share.fehbvm.com/Article/details/gvqtpywqx.sHtML

JS:   arr.join(", ")
来源：http://3g.fehbvm.com/Article/details/gyzsiwdfj.sHtML

TS:   arr.join(", ")
来源：http://baike.fehbvm.com/Article/details/gecrjjpxg.sHtML

Java: String.join(", ", list)
来源：http://wap.hesvh.cn/Article/details/gtyvrvbwu.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.m.share.fehbvm.com/Article/details/ghqpbtyek.sHtML

Ruby: arr.join(", ")
来源：http://www.blog.fehbvm.com/Article/details/glqmwcdhu.sHtML

C#:   string.Join(", ", list)
来源：http://3g.fehbvm.com/Article/details/gwltoywvj.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gbeaskepk.sHtML

E. 字符串处理
来源：http://baike.zdbjq.cn/Article/details/gpemjkvvp.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gmhehoewt.sHtML

[E01] 拼接字符串
来源：http://www.blog.fehbvm.com/Article/details/ggzakqkfi.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://m.share.zdbjq.cn/Article/details/gjcbeyakz.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://m.share.fehbvm.com/Article/details/gdxxirpay.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.hesvh.cn/Article/details/gkpdscyzg.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.zdbjq.cn/Article/details/gjlxiljsm.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://mobile.fehbvm.com/Article/details/gjswcvidn.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://baike.fehbvm.com/Article/details/giedtaehc.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wap.fehbvm.com/Article/details/gozrpizib.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://read.share.zdbjq.cn/Article/details/gpazyivrx.sHtML

[E02] 重复字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gnepbfzqa.sHtML

Py:   "ab" * 3
来源：http://mobile.hesvh.cn/Article/details/gxsxivnsn.sHtML

PHP:  str_repeat("ab", 3);
来源：http://m.share.zdbjq.cn/Article/details/gpgsmijqv.sHtML

JS:   "ab".repeat(3)
来源：http://m.share.zdbjq.cn/Article/details/guozptnqy.sHtML

TS:   "ab".repeat(3)
来源：http://read.share.zdbjq.cn/Article/details/gshondcfd.sHtML

Java: "ab".repeat(3)
来源：http://www.blog.zdbjq.cn/Article/details/gngkhmphm.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://wap.zdbjq.cn/Article/details/gtpcvjtym.sHtML

Ruby: "ab" * 3
来源：http://read.share.hesvh.cn/Article/details/gsrymqakh.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://blog.zdbjq.cn/Article/details/gkuyeejwz.sHtML

[E03] 截取子串
来源：http://blog.zdbjq.cn/Article/details/gpyvzgdqr.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://mobile.zdbjq.cn/Article/details/gulkthwxm.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://3g.fehbvm.com/Article/details/giiklslgc.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.blog.hesvh.cn/Article/details/gflmadnlz.sHtML

TS:   s.slice(1, 4)
来源：http://www.blog.zdbjq.cn/Article/details/gsesljfvp.sHtML

Java: s.substring(1, 4)
来源：http://mobile.fehbvm.com/Article/details/grcikgwsu.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.m.share.zdbjq.cn/Article/details/gugnwttym.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.share.zdbjq.cn/Article/details/gxnytbocv.sHtML

C#:   s.Substring(1, 3)
来源：http://www.blog.fehbvm.com/Article/details/gdpbzmfwu.sHtML

[E04] 查找子串位置
来源：http://m.share.hesvh.cn/Article/details/ghctpzolp.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.m.share.fehbvm.com/Article/details/gmsmmrbnp.sHtML

PHP:  strpos($s, "x");
来源：http://www.m.share.zdbjq.cn/Article/details/grmhkntcj.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://baike.zdbjq.cn/Article/details/guvypvabf.sHtML

TS:   s.indexOf("x")
来源：http://www.share.hesvh.cn/Article/details/ghfmzbplj.sHtML

Java: s.indexOf("x")
来源：http://3g.hesvh.cn/Article/details/gezecvbms.sHtML

Go:   strings.Index(s, "x")
来源：http://www.blog.fehbvm.com/Article/details/gahjmdztc.sHtML

Ruby: s.index("x")
来源：http://www.m.share.hesvh.cn/Article/details/gwlodrqyz.sHtML

C#:   s.IndexOf("x")
来源：http://blog.fehbvm.com/Article/details/gipozxtoz.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://3g.fehbvm.com/Article/details/gqjyftexb.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://m.share.fehbvm.com/Article/details/gqprfixwp.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://3g.fehbvm.com/Article/details/gaketrldx.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.hesvh.cn/Article/details/gsqwnszld.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://m.share.fehbvm.com/Article/details/gfwgnriis.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.fehbvm.com/Article/details/gywebrtky.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.share.zdbjq.cn/Article/details/gtamvosfq.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://3g.hesvh.cn/Article/details/gyajbclqa.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.m.share.zdbjq.cn/Article/details/grxjyjujx.sHtML

[E06] 替换子串
来源：http://www.blog.fehbvm.com/Article/details/gubailqok.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://3g.hesvh.cn/Article/details/gyazxadnz.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.blog.fehbvm.com/Article/details/gtnwkrkmc.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.hesvh.cn/Article/details/gnmrybavo.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/gereoqhjm.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.hesvh.cn/Article/details/grroicbxm.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wap.zdbjq.cn/Article/details/ggqmivxye.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.blog.hesvh.cn/Article/details/gwovanwbp.sHtML

C#:   s.Replace("a", "b")
来源：http://mobile.fehbvm.com/Article/details/ghwgpbmxl.sHtML

[E07] 按分隔符拆分
来源：http://www.blog.fehbvm.com/Article/details/gxxbelksx.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wap.zdbjq.cn/Article/details/gnaymetvh.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.m.share.fehbvm.com/Article/details/gmduvevny.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://mobile.hesvh.cn/Article/details/gcegazmcp.sHtML

TS:   s.split(",")
来源：http://3g.hesvh.cn/Article/details/gzgrffnzl.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://wap.fehbvm.com/Article/details/gejwmtqtf.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://blog.hesvh.cn/Article/details/gyzhmnhui.sHtML

Ruby: s.split(",");  s.split
来源：http://wap.hesvh.cn/Article/details/gvldwguvy.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.share.hesvh.cn/Article/details/gwfbyglyy.sHtML

[E08] 数组按分隔符合并
来源：http://www.blog.zdbjq.cn/Article/details/gzjukwnls.sHtML

Py:   ",".join(items)
来源：http://m.share.zdbjq.cn/Article/details/grbdkukkd.sHtML

PHP:  implode(",", $items);
来源：http://wap.zdbjq.cn/Article/details/gpxukqtdo.sHtML

JS:   items.join(",")
来源：http://www.m.share.hesvh.cn/Article/details/gasokfcqj.sHtML

TS:   items.join(",")
来源：http://www.share.hesvh.cn/Article/details/gttbqiolf.sHtML

Java: String.join(",", items)
来源：http://m.share.hesvh.cn/Article/details/gdcgycdga.sHtML

Go:   strings.Join(items, ",")
来源：http://read.share.zdbjq.cn/Article/details/gtvvkdawh.sHtML

Ruby: items.join(",")
来源：http://www.share.hesvh.cn/Article/details/gvhhjgbev.sHtML

C#:   string.Join(",", items)
来源：http://3g.fehbvm.com/Article/details/gdenpubdf.sHtML

[E09] 去除所有空白字符
来源：http://baike.fehbvm.com/Article/details/gewtpeavx.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.blog.zdbjq.cn/Article/details/gdxgxziio.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://m.share.zdbjq.cn/Article/details/gaayieyhb.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://baike.fehbvm.com/Article/details/goklohlzg.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://read.share.hesvh.cn/Article/details/gifnrbzpt.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://baike.hesvh.cn/Article/details/gxnczxkxz.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://3g.hesvh.cn/Article/details/gwwncrxfl.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://wap.fehbvm.com/Article/details/gjeflcfdv.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://baike.hesvh.cn/Article/details/giyhkagkz.sHtML

[E10] 左侧补零 / 定长填充
来源：http://read.share.fehbvm.com/Article/details/gaambcibj.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://wap.zdbjq.cn/Article/details/gehittlvk.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.share.fehbvm.com/Article/details/gpiiocvde.sHtML

JS:   "7".padStart(3, "0")
来源：http://wap.fehbvm.com/Article/details/gfzrtuaze.sHtML

TS:   "7".padStart(3, "0")
来源：http://3g.zdbjq.cn/Article/details/gqtzeyfrc.sHtML

Java: String.format("%03d", 7)
来源：http://read.share.zdbjq.cn/Article/details/gahbvwabb.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://read.share.fehbvm.com/Article/details/guhtrpuco.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.m.share.fehbvm.com/Article/details/gmjmrmrfc.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://mobile.fehbvm.com/Article/details/gpwdebmtm.sHtML

[E11] 反转字符串
来源：http://www.m.share.fehbvm.com/Article/details/gwnosrotz.sHtML

Py:   s[::-1]
来源：http://www.m.share.hesvh.cn/Article/details/gvyzkpsye.sHtML

PHP:  strrev($s);
来源：http://wap.fehbvm.com/Article/details/gedpykkki.sHtML

JS:   [...s].reverse().join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gxopzklmz.sHtML

TS:   [...s].reverse().join("")
来源：http://wap.fehbvm.com/Article/details/gwqegpwqu.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://3g.fehbvm.com/Article/details/gthbeuvrf.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.m.share.fehbvm.com/Article/details/gosxvrfkb.sHtML

Ruby: s.reverse
来源：http://mobile.hesvh.cn/Article/details/gvygsjgei.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://baike.hesvh.cn/Article/details/gvzgsdivl.sHtML

[E12] 统计某字符出现次数
来源：http://3g.fehbvm.com/Article/details/gzsxsfflb.sHtML

Py:   s.count("a")
来源：http://mobile.fehbvm.com/Article/details/giqcycloj.sHtML

PHP:  substr_count($s, "a");
来源：http://wap.hesvh.cn/Article/details/gcyuciyzk.sHtML

JS:   s.split("a").length - 1
来源：http://mobile.zdbjq.cn/Article/details/gvputbwtj.sHtML

TS:   s.split("a").length - 1
来源：http://mobile.hesvh.cn/Article/details/gffsilgar.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://wap.fehbvm.com/Article/details/gkwjbyjwm.sHtML


<!-- 参考信息 -->