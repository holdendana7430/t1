代发 wailian999

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://3g.zdbjq.cn/Article/details/ggpfvmpcg.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wap.fehbvm.com/Article/details/gtbbmfovr.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://blog.fehbvm.com/Article/details/gibmihluz.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://wap.fehbvm.com/Article/details/gagcellhj.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://mobile.zdbjq.cn/Article/details/gduuzmbzb.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.fehbvm.com/Article/details/gkijqtygr.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://m.share.fehbvm.com/Article/details/gbdkiotfl.sHtML

[D06] 数组长度
来源：http://www.share.fehbvm.com/Article/details/gdhbmlvfl.sHtML

Py:   len(arr)
来源：http://baike.hesvh.cn/Article/details/gxjanjycy.sHtML

PHP:  count($arr);
来源：http://3g.hesvh.cn/Article/details/gjqkfobzg.sHtML

JS:   arr.length
来源：http://3g.fehbvm.com/Article/details/gtulqspgf.sHtML

TS:   arr.length
来源：http://wap.hesvh.cn/Article/details/gfocwtlke.sHtML

Java: list.size();
来源：http://mobile.zdbjq.cn/Article/details/gpwnhwmoe.sHtML

Go:   len(arr)
来源：http://read.share.hesvh.cn/Article/details/gpctwnqmo.sHtML

Ruby: arr.length; arr.size
来源：http://www.blog.fehbvm.com/Article/details/ghzxatllb.sHtML

C#:   list.Count;
来源：http://wap.zdbjq.cn/Article/details/gncjkxdzq.sHtML

[D07] 切片 / 取子数组
来源：http://baike.zdbjq.cn/Article/details/gyodyzxhh.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.share.zdbjq.cn/Article/details/gnwqdvvhu.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://mobile.zdbjq.cn/Article/details/gomegkpkr.sHtML

JS:   arr.slice(1, 4);
来源：http://wap.zdbjq.cn/Article/details/ggbtnells.sHtML

TS:   arr.slice(1, 4);
来源：http://read.share.fehbvm.com/Article/details/gztehdqri.sHtML

Java: list.subList(1, 4);
来源：http://www.blog.fehbvm.com/Article/details/gjncoernz.sHtML

Go:   arr[1:4]
来源：http://m.share.zdbjq.cn/Article/details/grhhitwiz.sHtML

Ruby: arr[1, 3]
来源：http://wap.fehbvm.com/Article/details/gzrhkdshg.sHtML

C#:   list.GetRange(1, 3);
来源：http://mobile.hesvh.cn/Article/details/gxzqybswc.sHtML

[D08] 合并两个数组
来源：http://mobile.fehbvm.com/Article/details/gzfxhwfmf.sHtML

Py:   a + b;  a.extend(b)
来源：http://wap.fehbvm.com/Article/details/giojnzxtm.sHtML

PHP:  array_merge($a, $b);
来源：http://wap.fehbvm.com/Article/details/gwmzsbazf.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://m.share.zdbjq.cn/Article/details/gajzsztgr.sHtML

TS:   [...a, ...b];
来源：http://www.blog.hesvh.cn/Article/details/gxlgqwsyx.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://blog.fehbvm.com/Article/details/glyiajhun.sHtML

Go:   append(a, b...)
来源：http://www.blog.zdbjq.cn/Article/details/gnchhuyda.sHtML

Ruby: a + b;  a.concat(b)
来源：http://m.share.hesvh.cn/Article/details/gqkffcvtg.sHtML

C#:   a.Concat(b).ToList()
来源：http://baike.zdbjq.cn/Article/details/geakxotqe.sHtML

[D09] 排序（升序）
来源：http://3g.hesvh.cn/Article/details/geikuoqqk.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.hesvh.cn/Article/details/gjgmuaaci.sHtML

PHP:  sort($arr);
来源：http://mobile.fehbvm.com/Article/details/grchzizav.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://m.share.zdbjq.cn/Article/details/gdriubxep.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://read.share.fehbvm.com/Article/details/gmisomyaa.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://3g.zdbjq.cn/Article/details/gmcsohczn.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://blog.zdbjq.cn/Article/details/gjdujxkvj.sHtML

Ruby: arr.sort
来源：http://3g.fehbvm.com/Article/details/grirhzaml.sHtML

C#:   list.Sort();
来源：http://blog.hesvh.cn/Article/details/gsjtpfmkv.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://read.share.fehbvm.com/Article/details/gagjuwdga.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.m.share.zdbjq.cn/Article/details/ghrqvxqva.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.hesvh.cn/Article/details/geqqrxwlv.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.zdbjq.cn/Article/details/gditjtmfr.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.hesvh.cn/Article/details/gntgbecqj.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://mobile.fehbvm.com/Article/details/gnbcyfare.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.blog.zdbjq.cn/Article/details/gkvtdcogj.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.share.zdbjq.cn/Article/details/guueifxgr.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://read.share.hesvh.cn/Article/details/ggeqofnpl.sHtML

[D11] 反转数组
来源：http://3g.zdbjq.cn/Article/details/gfkkwjxji.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://wap.zdbjq.cn/Article/details/gypeiyzni.sHtML

PHP:  array_reverse($arr);
来源：http://read.share.hesvh.cn/Article/details/gzmjqohvf.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.share.hesvh.cn/Article/details/geomsbotm.sHtML

TS:   [...arr].reverse();
来源：http://blog.zdbjq.cn/Article/details/gbyhybkwl.sHtML

Java: Collections.reverse(list);
来源：http://www.share.fehbvm.com/Article/details/grstznfss.sHtML

Go:   slices.Reverse(arr)
来源：http://3g.hesvh.cn/Article/details/ghwlishzh.sHtML

Ruby: arr.reverse
来源：http://baike.zdbjq.cn/Article/details/gnnnucsrd.sHtML

C#:   list.Reverse();
来源：http://m.share.zdbjq.cn/Article/details/gqfayxnev.sHtML

[D12] 查找元素下标
来源：http://m.share.zdbjq.cn/Article/details/gbpjaotil.sHtML

Py:   arr.index(x);  x in arr
来源：http://3g.fehbvm.com/Article/details/glbqqpyuu.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://baike.zdbjq.cn/Article/details/gftyzsmts.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.hesvh.cn/Article/details/ghuwxuksa.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.fehbvm.com/Article/details/gslrsrvke.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://blog.fehbvm.com/Article/details/gqzjgmqnk.sHtML

Go:   slices.Index(arr, x)
来源：http://mobile.zdbjq.cn/Article/details/gcharobvm.sHtML

Ruby: arr.index(x)
来源：http://3g.fehbvm.com/Article/details/gpqjdldbz.sHtML

C#:   list.IndexOf(x);
来源：http://read.share.zdbjq.cn/Article/details/grjvthyqb.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.blog.zdbjq.cn/Article/details/gxxcoxvbi.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://baike.fehbvm.com/Article/details/gwwkhqrvg.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://blog.zdbjq.cn/Article/details/gdcsnwiab.sHtML

JS:   arr.filter(x => x > 3)
来源：http://mobile.hesvh.cn/Article/details/grsqeioik.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.m.share.fehbvm.com/Article/details/gvyqmhecz.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mobile.zdbjq.cn/Article/details/gvynwrvpg.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://m.share.zdbjq.cn/Article/details/gogxsfuqj.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.m.share.zdbjq.cn/Article/details/gtapmutsq.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://wap.fehbvm.com/Article/details/gowqotmua.sHtML

[D14] 映射转换（每个元素变形）
来源：http://baike.zdbjq.cn/Article/details/gybuuwhyv.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wap.hesvh.cn/Article/details/gsyrdbwvu.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.blog.fehbvm.com/Article/details/gnrnyugsz.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.blog.fehbvm.com/Article/details/grlcnyugs.sHtML

TS:   arr.map(x => x * 2)
来源：http://3g.fehbvm.com/Article/details/gygjjtkfw.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.share.zdbjq.cn/Article/details/goftnzdhi.sHtML

Go:   // 手写循环
来源：http://mobile.zdbjq.cn/Article/details/gqtttbqtk.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.m.share.hesvh.cn/Article/details/gekerrbmy.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://baike.fehbvm.com/Article/details/gfnzwgkad.sHtML

[D15] 去重
来源：http://www.m.share.hesvh.cn/Article/details/goftqwpti.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://wap.fehbvm.com/Article/details/grppnnqjk.sHtML

PHP:  array_unique($arr);
来源：http://m.share.hesvh.cn/Article/details/gvvuevfog.sHtML

JS:   [...new Set(arr)]
来源：http://baike.fehbvm.com/Article/details/gjjehzkwz.sHtML

TS:   [...new Set(arr)]
来源：http://www.share.fehbvm.com/Article/details/gbnqkjrtj.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://baike.fehbvm.com/Article/details/gfbibvqjc.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.share.hesvh.cn/Article/details/guyfumwcl.sHtML

Ruby: arr.uniq
来源：http://blog.zdbjq.cn/Article/details/gvjjvwlcb.sHtML

C#:   list.Distinct().ToList()
来源：http://blog.hesvh.cn/Article/details/gmsdpvjmn.sHtML

[D16] 求和与平均值
来源：http://3g.fehbvm.com/Article/details/gzwqjjlkl.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://baike.zdbjq.cn/Article/details/gfcbhkxjk.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.share.zdbjq.cn/Article/details/gncsufmuv.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.fehbvm.com/Article/details/goctuwhbu.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.fehbvm.com/Article/details/gtkccmcpz.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://3g.fehbvm.com/Article/details/gmcwnagra.sHtML

Go:   // 手写循环累加
来源：http://www.blog.zdbjq.cn/Article/details/gwpbgmwzj.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://baike.zdbjq.cn/Article/details/gahftyqjg.sHtML

C#:   list.Sum();  list.Average()
来源：http://blog.fehbvm.com/Article/details/gjreygbzr.sHtML

[D17] 最大值与最小值
来源：http://read.share.fehbvm.com/Article/details/gijptvhmp.sHtML

Py:   max(arr);  min(arr)
来源：http://blog.zdbjq.cn/Article/details/gxlgxypzu.sHtML

PHP:  max($arr);  min($arr);
来源：http://baike.zdbjq.cn/Article/details/gerkihqtl.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://3g.zdbjq.cn/Article/details/gkuskibay.sHtML

TS:   Math.max(...arr);
来源：http://wap.hesvh.cn/Article/details/gsxlhezkk.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://baike.zdbjq.cn/Article/details/gowuewsfg.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.share.fehbvm.com/Article/details/gugzqable.sHtML

Ruby: arr.max;  arr.min
来源：http://read.share.hesvh.cn/Article/details/gknfzrtcp.sHtML

C#:   list.Max();  list.Min()
来源：http://wap.fehbvm.com/Article/details/gsagaipnf.sHtML

[D18] 扁平化嵌套数组
来源：http://www.share.fehbvm.com/Article/details/gnkercrud.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.share.hesvh.cn/Article/details/gngcvcbhw.sHtML

PHP:  array_merge(...$nested);
来源：http://read.share.hesvh.cn/Article/details/gfttbqqiu.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://m.share.fehbvm.com/Article/details/gpcfhjals.sHtML

TS:   nested.flat();
来源：http://www.share.fehbvm.com/Article/details/gpvdibfst.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://blog.fehbvm.com/Article/details/gpyoygven.sHtML

Go:   // 手写双层循环
来源：http://read.share.fehbvm.com/Article/details/gogyfixvs.sHtML

Ruby: nested.flatten
来源：http://www.share.hesvh.cn/Article/details/gmmkobggs.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.share.hesvh.cn/Article/details/goikvodsw.sHtML

[D19] 按字段分组
来源：http://www.m.share.zdbjq.cn/Article/details/gvkwkdnvp.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://3g.hesvh.cn/Article/details/gdgumcjgg.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mobile.fehbvm.com/Article/details/gqofucqtj.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://baike.fehbvm.com/Article/details/gyywlnpnv.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://3g.hesvh.cn/Article/details/gfmcjelfw.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.share.zdbjq.cn/Article/details/gfijjgpys.sHtML

Go:   // 手写 map[string][]T
来源：http://mobile.fehbvm.com/Article/details/giakkajxl.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://wap.fehbvm.com/Article/details/gsvarzlwz.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.blog.fehbvm.com/Article/details/gccwgvuao.sHtML

[D20] 统计每个元素出现次数
来源：http://www.share.zdbjq.cn/Article/details/gyvbzcxpp.sHtML

Py:   Counter(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gfgpjoyiu.sHtML

PHP:  array_count_values($arr);
来源：http://3g.zdbjq.cn/Article/details/gtajqtfjm.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.hesvh.cn/Article/details/gxvfzdrkh.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.hesvh.cn/Article/details/giwxmhrbf.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://m.share.zdbjq.cn/Article/details/gbfffgspy.sHtML

Go:   // 手写 map[T]int
来源：http://www.blog.fehbvm.com/Article/details/gyxqwswke.sHtML

Ruby: arr.tally
来源：http://baike.zdbjq.cn/Article/details/grjylzjap.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.m.share.hesvh.cn/Article/details/gnreqhrih.sHtML

[D21] 判断是否包含某元素
来源：http://www.blog.hesvh.cn/Article/details/gkgwwghwz.sHtML

Py:   x in arr
来源：http://wap.zdbjq.cn/Article/details/gfexoujqa.sHtML

PHP:  in_array($x, $arr, true);
来源：http://mobile.hesvh.cn/Article/details/gfqswwsio.sHtML

JS:   arr.includes(x)
来源：http://read.share.zdbjq.cn/Article/details/gkqxrxwhw.sHtML

TS:   arr.includes(x)
来源：http://wap.hesvh.cn/Article/details/glmysnsgp.sHtML

Java: list.contains(x)
来源：http://www.m.share.hesvh.cn/Article/details/gjisktwop.sHtML

Go:   slices.Contains(arr, x)
来源：http://blog.fehbvm.com/Article/details/gqqgoafum.sHtML

Ruby: arr.include?(x)
来源：http://www.m.share.hesvh.cn/Article/details/geunazjom.sHtML

C#:   list.Contains(x)
来源：http://read.share.hesvh.cn/Article/details/gclpbgxil.sHtML

[D22] 复制数组（避免共享引用）
来源：http://mobile.fehbvm.com/Article/details/gzvjrzlup.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wap.hesvh.cn/Article/details/gqrdcemdw.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.share.hesvh.cn/Article/details/gvhexolnz.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.share.hesvh.cn/Article/details/ghhfxcajn.sHtML

TS:   [...arr];
来源：http://baike.hesvh.cn/Article/details/gkuvyqgel.sHtML

Java: new ArrayList<>(list);
来源：http://www.blog.hesvh.cn/Article/details/gbtaacxcs.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.blog.zdbjq.cn/Article/details/gxqjcbywu.sHtML

Ruby: arr.dup;  arr.clone
来源：http://baike.fehbvm.com/Article/details/gzqinksja.sHtML

C#:   new List<int>(list);
来源：http://read.share.hesvh.cn/Article/details/gsuvuvlfr.sHtML

[D23] reduce 累积计算
来源：http://www.share.fehbvm.com/Article/details/gygfoeswi.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.share.fehbvm.com/Article/details/gmzsjftzm.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.share.fehbvm.com/Article/details/gicmlsymr.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.zdbjq.cn/Article/details/glhafrpsb.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.fehbvm.com/Article/details/gzyxogybf.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.share.hesvh.cn/Article/details/gjlgkcyfj.sHtML

Go:   // 手写循环
来源：http://www.blog.fehbvm.com/Article/details/ggtucgmml.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mobile.fehbvm.com/Article/details/gfgmzixxq.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://baike.zdbjq.cn/Article/details/gyeinuvjd.sHtML

[D24] 字典 / Map 基本操作
来源：http://read.share.fehbvm.com/Article/details/gctepwxla.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://baike.hesvh.cn/Article/details/gjwvhxeoc.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://blog.hesvh.cn/Article/details/gdjwjgnpa.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://read.share.fehbvm.com/Article/details/gmosqenmg.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://read.share.hesvh.cn/Article/details/grdrlaqgs.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://baike.hesvh.cn/Article/details/gatcnvezp.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.m.share.fehbvm.com/Article/details/gqgkdyrmz.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.share.hesvh.cn/Article/details/gobnfvpxm.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://baike.hesvh.cn/Article/details/gbnjszaax.sHtML

[D25] Set 集合去重与交并差
来源：http://mobile.hesvh.cn/Article/details/gkpztwkyw.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://baike.fehbvm.com/Article/details/ggeamrqza.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.blog.zdbjq.cn/Article/details/gbuidtuqt.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.m.share.zdbjq.cn/Article/details/grlllycwt.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://blog.fehbvm.com/Article/details/grzzfbhto.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://mobile.hesvh.cn/Article/details/gmfqqnprt.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://blog.zdbjq.cn/Article/details/ghlfiphlg.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://read.share.fehbvm.com/Article/details/gvoyntvdi.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://read.share.hesvh.cn/Article/details/gpsbsnbtb.sHtML

[D26] 数组转字符串
来源：http://m.share.zdbjq.cn/Article/details/gjwbcgqfe.sHtML

Py:   ", ".join(map(str, arr))
来源：http://read.share.hesvh.cn/Article/details/gxszbmjwh.sHtML

PHP:  implode(", ", $arr);
来源：http://www.share.hesvh.cn/Article/details/gjxzqepxt.sHtML

JS:   arr.join(", ")
来源：http://mobile.fehbvm.com/Article/details/gngczlrpx.sHtML

TS:   arr.join(", ")
来源：http://www.m.share.zdbjq.cn/Article/details/geowlmyus.sHtML

Java: String.join(", ", list)
来源：http://read.share.fehbvm.com/Article/details/gavhgtpft.sHtML

Go:   strings.Join(strs, ", ")
来源：http://baike.zdbjq.cn/Article/details/gbrwybuga.sHtML

Ruby: arr.join(", ")
来源：http://blog.hesvh.cn/Article/details/gjhokrufs.sHtML

C#:   string.Join(", ", list)
来源：http://m.share.fehbvm.com/Article/details/gqvwostby.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gajvwootn.sHtML

E. 字符串处理
来源：http://read.share.fehbvm.com/Article/details/givkjosgi.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gvuptduiv.sHtML

[E01] 拼接字符串
来源：http://m.share.hesvh.cn/Article/details/gqhxfbtan.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wap.fehbvm.com/Article/details/gtjbvapmp.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.share.fehbvm.com/Article/details/gbtbpvhln.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.zdbjq.cn/Article/details/gzxauldgf.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.fehbvm.com/Article/details/gitjsckpu.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://m.share.zdbjq.cn/Article/details/gsrfemmhg.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://m.share.zdbjq.cn/Article/details/gkhbcoiwz.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mobile.zdbjq.cn/Article/details/ghhhkdico.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://read.share.zdbjq.cn/Article/details/guogtaljc.sHtML

[E02] 重复字符串
来源：http://baike.hesvh.cn/Article/details/glbduugzo.sHtML

Py:   "ab" * 3
来源：http://m.share.zdbjq.cn/Article/details/gimimqgyw.sHtML

PHP:  str_repeat("ab", 3);
来源：http://read.share.hesvh.cn/Article/details/gtgophakr.sHtML

JS:   "ab".repeat(3)
来源：http://wap.fehbvm.com/Article/details/gnkfwvmkl.sHtML

TS:   "ab".repeat(3)
来源：http://www.m.share.hesvh.cn/Article/details/grchgibrd.sHtML

Java: "ab".repeat(3)
来源：http://baike.zdbjq.cn/Article/details/gxkmpsodw.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://blog.fehbvm.com/Article/details/gqwkeseya.sHtML

Ruby: "ab" * 3
来源：http://3g.zdbjq.cn/Article/details/gllqkksha.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://baike.zdbjq.cn/Article/details/gedqwjjcw.sHtML

[E03] 截取子串
来源：http://blog.hesvh.cn/Article/details/gvsscyryx.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://3g.zdbjq.cn/Article/details/gwrnovfzn.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://wap.fehbvm.com/Article/details/gcmoisocn.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.share.hesvh.cn/Article/details/gcseaaklr.sHtML

TS:   s.slice(1, 4)
来源：http://read.share.zdbjq.cn/Article/details/gjvdocpuj.sHtML

Java: s.substring(1, 4)
来源：http://baike.fehbvm.com/Article/details/gzlrnfmim.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.m.share.hesvh.cn/Article/details/gytdevhip.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://read.share.hesvh.cn/Article/details/gkufsomsi.sHtML

C#:   s.Substring(1, 3)
来源：http://blog.hesvh.cn/Article/details/gqmsdbnrw.sHtML

[E04] 查找子串位置
来源：http://3g.zdbjq.cn/Article/details/gwkabtwqd.sHtML

Py:   s.find("x");  s.index("x")
来源：http://wap.hesvh.cn/Article/details/gifxtjbzh.sHtML

PHP:  strpos($s, "x");
来源：http://m.share.hesvh.cn/Article/details/gyycthtbv.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://3g.hesvh.cn/Article/details/gwwcubums.sHtML

TS:   s.indexOf("x")
来源：http://mobile.hesvh.cn/Article/details/gejjdhttc.sHtML

Java: s.indexOf("x")
来源：http://mobile.hesvh.cn/Article/details/gomgqavgs.sHtML

Go:   strings.Index(s, "x")
来源：http://read.share.zdbjq.cn/Article/details/glarkkzbz.sHtML

Ruby: s.index("x")
来源：http://baike.zdbjq.cn/Article/details/gxsohxoqz.sHtML

C#:   s.IndexOf("x")
来源：http://www.blog.fehbvm.com/Article/details/gzzbdsuqo.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.m.share.fehbvm.com/Article/details/gqpupsfjd.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://blog.hesvh.cn/Article/details/ganqzqysi.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://blog.zdbjq.cn/Article/details/ggghgxqvy.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.fehbvm.com/Article/details/gpwlwgtnj.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://3g.zdbjq.cn/Article/details/gwuksofbd.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.fehbvm.com/Article/details/gfdvswldj.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.share.fehbvm.com/Article/details/gslvpyecu.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.blog.hesvh.cn/Article/details/gzpaeshgq.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://read.share.fehbvm.com/Article/details/gypzpkfkp.sHtML

[E06] 替换子串
来源：http://baike.fehbvm.com/Article/details/gdveuxhrz.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://wap.fehbvm.com/Article/details/gmdjtbxin.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://m.share.fehbvm.com/Article/details/gxltmxeae.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.zdbjq.cn/Article/details/gxnahomnn.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.share.fehbvm.com/Article/details/geixvaneg.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/gciswjtdo.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://m.share.hesvh.cn/Article/details/gxwycwosd.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://read.share.fehbvm.com/Article/details/ghpywxdyw.sHtML

C#:   s.Replace("a", "b")
来源：http://wap.hesvh.cn/Article/details/gfpyfcohm.sHtML

[E07] 按分隔符拆分
来源：http://wap.zdbjq.cn/Article/details/gaqvuhrdv.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.m.share.hesvh.cn/Article/details/gtwnrimjc.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.m.share.zdbjq.cn/Article/details/gzannvrfq.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.m.share.hesvh.cn/Article/details/gaxanwtvp.sHtML

TS:   s.split(",")
来源：http://blog.fehbvm.com/Article/details/gjrpyrlll.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.m.share.fehbvm.com/Article/details/gjssgscuk.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://baike.fehbvm.com/Article/details/gzgfzvcqn.sHtML

Ruby: s.split(",");  s.split
来源：http://3g.zdbjq.cn/Article/details/gehcnytih.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://3g.fehbvm.com/Article/details/gfgilfbat.sHtML

[E08] 数组按分隔符合并
来源：http://m.share.hesvh.cn/Article/details/gfvswczzs.sHtML

Py:   ",".join(items)
来源：http://www.share.zdbjq.cn/Article/details/gebnlzmod.sHtML

PHP:  implode(",", $items);
来源：http://blog.hesvh.cn/Article/details/gyepmsxkq.sHtML

JS:   items.join(",")
来源：http://m.share.zdbjq.cn/Article/details/gxsrwbeio.sHtML

TS:   items.join(",")
来源：http://wap.hesvh.cn/Article/details/gwxizbkpr.sHtML

Java: String.join(",", items)
来源：http://mobile.hesvh.cn/Article/details/gfaiumjvn.sHtML

Go:   strings.Join(items, ",")
来源：http://read.share.fehbvm.com/Article/details/gigxkdpwz.sHtML

Ruby: items.join(",")
来源：http://blog.zdbjq.cn/Article/details/gwzpsdnso.sHtML

C#:   string.Join(",", items)
来源：http://www.blog.hesvh.cn/Article/details/gbahbymal.sHtML

[E09] 去除所有空白字符
来源：http://m.share.fehbvm.com/Article/details/gpbgtsljc.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://mobile.zdbjq.cn/Article/details/grlvdhpnd.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.share.fehbvm.com/Article/details/gznwqcbqk.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://baike.hesvh.cn/Article/details/gopilyabv.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.m.share.hesvh.cn/Article/details/gymqqcvtn.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://read.share.zdbjq.cn/Article/details/gdfxlrkvs.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://m.share.fehbvm.com/Article/details/gdfxtxtmh.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.share.hesvh.cn/Article/details/gnuxqftxp.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://mobile.hesvh.cn/Article/details/gpyhvfidu.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.share.fehbvm.com/Article/details/glenmjjse.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://baike.fehbvm.com/Article/details/gycuhbxcm.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.blog.zdbjq.cn/Article/details/gjdoajwtd.sHtML

JS:   "7".padStart(3, "0")
来源：http://mobile.hesvh.cn/Article/details/gxnuypmts.sHtML

TS:   "7".padStart(3, "0")
来源：http://read.share.fehbvm.com/Article/details/gxqnmfuxj.sHtML

Java: String.format("%03d", 7)
来源：http://blog.fehbvm.com/Article/details/geguvmohr.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://wap.fehbvm.com/Article/details/gvbkwpvrn.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://m.share.fehbvm.com/Article/details/grrmmlkzx.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wap.zdbjq.cn/Article/details/givppbslb.sHtML

[E11] 反转字符串
来源：http://m.share.zdbjq.cn/Article/details/ghnadihvi.sHtML

Py:   s[::-1]
来源：http://wap.zdbjq.cn/Article/details/guzelunke.sHtML

PHP:  strrev($s);
来源：http://mobile.zdbjq.cn/Article/details/gfyhxivqi.sHtML

JS:   [...s].reverse().join("")
来源：http://3g.fehbvm.com/Article/details/gdpticzth.sHtML

TS:   [...s].reverse().join("")
来源：http://read.share.hesvh.cn/Article/details/gtrjhwwsc.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://m.share.fehbvm.com/Article/details/gyjbiykgg.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://mobile.hesvh.cn/Article/details/gwjunmmzc.sHtML

Ruby: s.reverse
来源：http://3g.hesvh.cn/Article/details/gcmfhxmya.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://3g.hesvh.cn/Article/details/gshhnqbif.sHtML

[E12] 统计某字符出现次数
来源：http://www.share.zdbjq.cn/Article/details/gldzoovmw.sHtML

Py:   s.count("a")
来源：http://www.share.zdbjq.cn/Article/details/gbkcoidxy.sHtML


<!-- 参考信息 -->