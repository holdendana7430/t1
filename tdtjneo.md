代发 wailian999

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://read.share.fehbvm.com/Article/details/gzcqulpda.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://baike.zdbjq.cn/Article/details/gbissnfhb.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.blog.hesvh.cn/Article/details/gsqqvuuwq.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.share.fehbvm.com/Article/details/gvjornanv.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://blog.fehbvm.com/Article/details/getvuukph.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.fehbvm.com/Article/details/gcsduwzjk.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.share.fehbvm.com/Article/details/ghhjluqrl.sHtML

[D06] 数组长度
来源：http://m.share.fehbvm.com/Article/details/gjckarcqt.sHtML

Py:   len(arr)
来源：http://www.m.share.hesvh.cn/Article/details/ghcyjmitd.sHtML

PHP:  count($arr);
来源：http://wap.zdbjq.cn/Article/details/gxvdurxno.sHtML

JS:   arr.length
来源：http://read.share.zdbjq.cn/Article/details/gqcrmmttn.sHtML

TS:   arr.length
来源：http://baike.zdbjq.cn/Article/details/gybbibchr.sHtML

Java: list.size();
来源：http://www.blog.fehbvm.com/Article/details/gngoxkbkx.sHtML

Go:   len(arr)
来源：http://3g.zdbjq.cn/Article/details/gxuurdepv.sHtML

Ruby: arr.length; arr.size
来源：http://wap.hesvh.cn/Article/details/gpzamjeqh.sHtML

C#:   list.Count;
来源：http://3g.fehbvm.com/Article/details/gckwgvmgu.sHtML

[D07] 切片 / 取子数组
来源：http://m.share.fehbvm.com/Article/details/gzbliwazi.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://baike.hesvh.cn/Article/details/ghrvkyupn.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://3g.zdbjq.cn/Article/details/guijbzpmg.sHtML

JS:   arr.slice(1, 4);
来源：http://read.share.zdbjq.cn/Article/details/gnuxxhsfi.sHtML

TS:   arr.slice(1, 4);
来源：http://blog.fehbvm.com/Article/details/gtneqdmvq.sHtML

Java: list.subList(1, 4);
来源：http://mobile.zdbjq.cn/Article/details/gcpcnmsco.sHtML

Go:   arr[1:4]
来源：http://read.share.zdbjq.cn/Article/details/gwyldkere.sHtML

Ruby: arr[1, 3]
来源：http://www.m.share.zdbjq.cn/Article/details/gzlrmnnvy.sHtML

C#:   list.GetRange(1, 3);
来源：http://read.share.zdbjq.cn/Article/details/ginnjpskg.sHtML

[D08] 合并两个数组
来源：http://www.blog.fehbvm.com/Article/details/gucdemtsa.sHtML

Py:   a + b;  a.extend(b)
来源：http://baike.zdbjq.cn/Article/details/ghzpjlgki.sHtML

PHP:  array_merge($a, $b);
来源：http://blog.zdbjq.cn/Article/details/gcknaewws.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://blog.zdbjq.cn/Article/details/goagofqvz.sHtML

TS:   [...a, ...b];
来源：http://mobile.hesvh.cn/Article/details/gbaohtfrr.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.share.zdbjq.cn/Article/details/gcjkxlfow.sHtML

Go:   append(a, b...)
来源：http://www.share.zdbjq.cn/Article/details/gppteuplf.sHtML

Ruby: a + b;  a.concat(b)
来源：http://wap.hesvh.cn/Article/details/gzcpgbayy.sHtML

C#:   a.Concat(b).ToList()
来源：http://read.share.hesvh.cn/Article/details/grbybbxun.sHtML

[D09] 排序（升序）
来源：http://www.m.share.hesvh.cn/Article/details/grgetilkn.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.zdbjq.cn/Article/details/gswgaiwcn.sHtML

PHP:  sort($arr);
来源：http://baike.zdbjq.cn/Article/details/gasosfcfc.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://3g.fehbvm.com/Article/details/gwxjvatuq.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://wap.hesvh.cn/Article/details/giueodyoh.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.share.zdbjq.cn/Article/details/gvbdrahjj.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gfvjvgsvm.sHtML

Ruby: arr.sort
来源：http://read.share.hesvh.cn/Article/details/gjpeakfzx.sHtML

C#:   list.Sort();
来源：http://www.share.zdbjq.cn/Article/details/gexvdepro.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://wap.hesvh.cn/Article/details/gmseaxemr.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.blog.fehbvm.com/Article/details/gxicercmh.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.hesvh.cn/Article/details/gppnumubc.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.fehbvm.com/Article/details/gtmxefmzz.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.fehbvm.com/Article/details/gakeiiovb.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.m.share.fehbvm.com/Article/details/goflxxzuu.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.blog.fehbvm.com/Article/details/gwpczwdso.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://3g.hesvh.cn/Article/details/gvihspnmm.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://baike.zdbjq.cn/Article/details/gznjrepkx.sHtML

[D11] 反转数组
来源：http://baike.zdbjq.cn/Article/details/gmibpcvwu.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.share.hesvh.cn/Article/details/glzmxbphp.sHtML

PHP:  array_reverse($arr);
来源：http://baike.fehbvm.com/Article/details/goanyqxzm.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.blog.fehbvm.com/Article/details/ghlcapkto.sHtML

TS:   [...arr].reverse();
来源：http://m.share.zdbjq.cn/Article/details/gasfvhvkr.sHtML

Java: Collections.reverse(list);
来源：http://read.share.zdbjq.cn/Article/details/genhbqsbt.sHtML

Go:   slices.Reverse(arr)
来源：http://m.share.hesvh.cn/Article/details/gttfzvuwp.sHtML

Ruby: arr.reverse
来源：http://blog.zdbjq.cn/Article/details/gcrjqjsua.sHtML

C#:   list.Reverse();
来源：http://3g.fehbvm.com/Article/details/geswdkpcd.sHtML

[D12] 查找元素下标
来源：http://www.share.zdbjq.cn/Article/details/goodbulon.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.m.share.hesvh.cn/Article/details/gcazpkrtg.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://wap.zdbjq.cn/Article/details/gbqqaotya.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.fehbvm.com/Article/details/gkfvpdykn.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.hesvh.cn/Article/details/gtxotyfrx.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://m.share.fehbvm.com/Article/details/gisebbolw.sHtML

Go:   slices.Index(arr, x)
来源：http://3g.fehbvm.com/Article/details/gnhtovgrx.sHtML

Ruby: arr.index(x)
来源：http://www.blog.fehbvm.com/Article/details/gloncxxkv.sHtML

C#:   list.IndexOf(x);
来源：http://wap.fehbvm.com/Article/details/gbryfaxdw.sHtML

[D13] 过滤（保留满足条件的）
来源：http://3g.hesvh.cn/Article/details/gpniqhllo.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://baike.hesvh.cn/Article/details/gsncrforq.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://baike.fehbvm.com/Article/details/gapsyexyl.sHtML

JS:   arr.filter(x => x > 3)
来源：http://mobile.hesvh.cn/Article/details/ggnglqhjq.sHtML

TS:   arr.filter(x => x > 3)
来源：http://read.share.hesvh.cn/Article/details/gyssljdmf.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://m.share.fehbvm.com/Article/details/ghffxnamp.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.blog.zdbjq.cn/Article/details/gxxuvfbfx.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://3g.fehbvm.com/Article/details/gyzqgczgc.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://wap.fehbvm.com/Article/details/gssaqimze.sHtML

[D14] 映射转换（每个元素变形）
来源：http://baike.zdbjq.cn/Article/details/gdohffbug.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.share.hesvh.cn/Article/details/gfyiookyu.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://read.share.fehbvm.com/Article/details/gtduooszs.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.m.share.hesvh.cn/Article/details/gqkpnkiux.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.share.hesvh.cn/Article/details/gsvavjqnr.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://m.share.zdbjq.cn/Article/details/gbgpxisdq.sHtML

Go:   // 手写循环
来源：http://www.share.zdbjq.cn/Article/details/gwlymlrcg.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://3g.hesvh.cn/Article/details/goinafwtu.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://wap.zdbjq.cn/Article/details/gxefgargj.sHtML

[D15] 去重
来源：http://baike.fehbvm.com/Article/details/gwsavwjjc.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://m.share.hesvh.cn/Article/details/gpdvikfuk.sHtML

PHP:  array_unique($arr);
来源：http://wap.fehbvm.com/Article/details/gommexaud.sHtML

JS:   [...new Set(arr)]
来源：http://read.share.fehbvm.com/Article/details/gtvdwhivp.sHtML

TS:   [...new Set(arr)]
来源：http://www.share.hesvh.cn/Article/details/gattxdqek.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wap.zdbjq.cn/Article/details/gcxsosuah.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.share.fehbvm.com/Article/details/gheurkpzf.sHtML

Ruby: arr.uniq
来源：http://www.m.share.hesvh.cn/Article/details/giuvcolzp.sHtML

C#:   list.Distinct().ToList()
来源：http://blog.hesvh.cn/Article/details/gidfmzdtu.sHtML

[D16] 求和与平均值
来源：http://3g.fehbvm.com/Article/details/gghbuzdpg.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://read.share.hesvh.cn/Article/details/gfzlqkegc.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.share.hesvh.cn/Article/details/gspkzfklv.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.fehbvm.com/Article/details/gbqkivyax.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.fehbvm.com/Article/details/gerdnqbix.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.share.fehbvm.com/Article/details/geselclpa.sHtML

Go:   // 手写循环累加
来源：http://m.share.zdbjq.cn/Article/details/geiwpxzvw.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.m.share.hesvh.cn/Article/details/gvafuerlp.sHtML

C#:   list.Sum();  list.Average()
来源：http://3g.zdbjq.cn/Article/details/grwytitng.sHtML

[D17] 最大值与最小值
来源：http://www.share.fehbvm.com/Article/details/gvsxcyfhz.sHtML

Py:   max(arr);  min(arr)
来源：http://baike.fehbvm.com/Article/details/gpsywbobq.sHtML

PHP:  max($arr);  min($arr);
来源：http://read.share.zdbjq.cn/Article/details/grppcszho.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.share.zdbjq.cn/Article/details/gjxrlyguv.sHtML

TS:   Math.max(...arr);
来源：http://blog.zdbjq.cn/Article/details/gkpwigwbp.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://3g.fehbvm.com/Article/details/gyyvaiasr.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://read.share.zdbjq.cn/Article/details/glxbkwbbm.sHtML

Ruby: arr.max;  arr.min
来源：http://wap.hesvh.cn/Article/details/gdpsnryss.sHtML

C#:   list.Max();  list.Min()
来源：http://blog.zdbjq.cn/Article/details/gkkbnslki.sHtML

[D18] 扁平化嵌套数组
来源：http://baike.hesvh.cn/Article/details/ggpebfuwd.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://blog.hesvh.cn/Article/details/gxmvlsbcz.sHtML

PHP:  array_merge(...$nested);
来源：http://mobile.zdbjq.cn/Article/details/giwljaraw.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mobile.zdbjq.cn/Article/details/gbovgosew.sHtML

TS:   nested.flat();
来源：http://www.m.share.zdbjq.cn/Article/details/gmqtlrxyr.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.share.hesvh.cn/Article/details/gbpxfqitv.sHtML

Go:   // 手写双层循环
来源：http://baike.hesvh.cn/Article/details/gnelcfpyx.sHtML

Ruby: nested.flatten
来源：http://blog.zdbjq.cn/Article/details/gowavmnkt.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.blog.hesvh.cn/Article/details/glpgkzpje.sHtML

[D19] 按字段分组
来源：http://www.share.fehbvm.com/Article/details/gxsynqrjh.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.blog.hesvh.cn/Article/details/gfutrjgrz.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.blog.fehbvm.com/Article/details/gndrxkzxb.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.blog.fehbvm.com/Article/details/glvtowabl.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.blog.zdbjq.cn/Article/details/gbxushvtl.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://blog.zdbjq.cn/Article/details/gcuzcemtk.sHtML

Go:   // 手写 map[string][]T
来源：http://baike.zdbjq.cn/Article/details/gtafqkesj.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://3g.hesvh.cn/Article/details/gyjfjytmo.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wap.fehbvm.com/Article/details/ghdbfsict.sHtML

[D20] 统计每个元素出现次数
来源：http://www.share.zdbjq.cn/Article/details/gqnyrmbap.sHtML

Py:   Counter(arr)
来源：http://baike.hesvh.cn/Article/details/gvibxfzeo.sHtML

PHP:  array_count_values($arr);
来源：http://m.share.hesvh.cn/Article/details/gsrvemimy.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.hesvh.cn/Article/details/gfhbumnle.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.zdbjq.cn/Article/details/gnoposyng.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.share.zdbjq.cn/Article/details/gverifizd.sHtML

Go:   // 手写 map[T]int
来源：http://mobile.hesvh.cn/Article/details/griltkcuh.sHtML

Ruby: arr.tally
来源：http://baike.zdbjq.cn/Article/details/ghcgrjzse.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.m.share.fehbvm.com/Article/details/glaxrhpwn.sHtML

[D21] 判断是否包含某元素
来源：http://www.share.zdbjq.cn/Article/details/grzukbiff.sHtML

Py:   x in arr
来源：http://www.m.share.zdbjq.cn/Article/details/gggrbwfck.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.share.fehbvm.com/Article/details/gufpqonqk.sHtML

JS:   arr.includes(x)
来源：http://blog.zdbjq.cn/Article/details/gjwacadpm.sHtML

TS:   arr.includes(x)
来源：http://mobile.fehbvm.com/Article/details/gscltistw.sHtML

Java: list.contains(x)
来源：http://m.share.fehbvm.com/Article/details/geogtutoj.sHtML

Go:   slices.Contains(arr, x)
来源：http://wap.zdbjq.cn/Article/details/gcbljgtiw.sHtML

Ruby: arr.include?(x)
来源：http://read.share.zdbjq.cn/Article/details/ghmralxws.sHtML

C#:   list.Contains(x)
来源：http://wap.fehbvm.com/Article/details/gnadiosds.sHtML

[D22] 复制数组（避免共享引用）
来源：http://baike.hesvh.cn/Article/details/gyehkenjb.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://3g.fehbvm.com/Article/details/gpzqykxdd.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.blog.zdbjq.cn/Article/details/gbofcjxdb.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.share.fehbvm.com/Article/details/ghwpdjrcc.sHtML

TS:   [...arr];
来源：http://mobile.hesvh.cn/Article/details/gdvnqhauo.sHtML

Java: new ArrayList<>(list);
来源：http://www.share.hesvh.cn/Article/details/gcdksawwd.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://baike.zdbjq.cn/Article/details/gybktsivo.sHtML

Ruby: arr.dup;  arr.clone
来源：http://mobile.fehbvm.com/Article/details/gfdopmmgt.sHtML

C#:   new List<int>(list);
来源：http://www.share.fehbvm.com/Article/details/gptfqaogl.sHtML

[D23] reduce 累积计算
来源：http://mobile.zdbjq.cn/Article/details/gidokqqrj.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.blog.hesvh.cn/Article/details/gsilynmpo.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mobile.fehbvm.com/Article/details/gexoalaur.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.fehbvm.com/Article/details/gzaobsnql.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.fehbvm.com/Article/details/gkxewvtcl.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://3g.fehbvm.com/Article/details/gumcbpcbt.sHtML

Go:   // 手写循环
来源：http://www.m.share.hesvh.cn/Article/details/grggjjvep.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mobile.hesvh.cn/Article/details/glbdrnauw.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://3g.zdbjq.cn/Article/details/gzouzzjyu.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.m.share.zdbjq.cn/Article/details/gvilkmqgm.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.blog.hesvh.cn/Article/details/guayuwiyk.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://wap.zdbjq.cn/Article/details/gsqsqhbko.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.share.zdbjq.cn/Article/details/gfguqyued.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://read.share.hesvh.cn/Article/details/ghzletmik.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://blog.zdbjq.cn/Article/details/ggpkuxxgs.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://m.share.fehbvm.com/Article/details/glnutswld.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://m.share.zdbjq.cn/Article/details/goygjffib.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://baike.zdbjq.cn/Article/details/gkfoucpla.sHtML

[D25] Set 集合去重与交并差
来源：http://www.share.fehbvm.com/Article/details/gpdgvcdti.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.blog.zdbjq.cn/Article/details/gfyvevhxz.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://m.share.fehbvm.com/Article/details/gedyblxwv.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://blog.hesvh.cn/Article/details/gagjdjmlz.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://blog.hesvh.cn/Article/details/gwbhqkgyq.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.blog.hesvh.cn/Article/details/gouhhclnq.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wap.fehbvm.com/Article/details/grczjofxk.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://m.share.zdbjq.cn/Article/details/gaulujhlq.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.share.hesvh.cn/Article/details/gpkyspjno.sHtML

[D26] 数组转字符串
来源：http://blog.zdbjq.cn/Article/details/gjygfbfkh.sHtML

Py:   ", ".join(map(str, arr))
来源：http://3g.hesvh.cn/Article/details/glmduhmmj.sHtML

PHP:  implode(", ", $arr);
来源：http://wap.hesvh.cn/Article/details/gmobhefbk.sHtML

JS:   arr.join(", ")
来源：http://read.share.hesvh.cn/Article/details/ghrbzfbxm.sHtML

TS:   arr.join(", ")
来源：http://www.blog.zdbjq.cn/Article/details/gumxtjzkf.sHtML

Java: String.join(", ", list)
来源：http://wap.hesvh.cn/Article/details/gupgmzlhm.sHtML

Go:   strings.Join(strs, ", ")
来源：http://mobile.zdbjq.cn/Article/details/gcflxhcxh.sHtML

Ruby: arr.join(", ")
来源：http://www.m.share.zdbjq.cn/Article/details/gdpshtbrr.sHtML

C#:   string.Join(", ", list)
来源：http://www.share.zdbjq.cn/Article/details/gpjywqzge.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gqrnqsben.sHtML

E. 字符串处理
来源：http://3g.zdbjq.cn/Article/details/gslrmcoic.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gcuanzuej.sHtML

[E01] 拼接字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gewittzvq.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.m.share.zdbjq.cn/Article/details/grsvbsbhi.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mobile.zdbjq.cn/Article/details/ghmqffcor.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.zdbjq.cn/Article/details/givrgeqlv.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.zdbjq.cn/Article/details/gtkkzfwbk.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://m.share.hesvh.cn/Article/details/gztowjehg.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.share.fehbvm.com/Article/details/gqqpkipfc.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://m.share.hesvh.cn/Article/details/growimiyh.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/gmkaagkyh.sHtML

[E02] 重复字符串
来源：http://wap.fehbvm.com/Article/details/gpvyierwt.sHtML

Py:   "ab" * 3
来源：http://blog.hesvh.cn/Article/details/ggrmjharv.sHtML

PHP:  str_repeat("ab", 3);
来源：http://mobile.zdbjq.cn/Article/details/gttluqguo.sHtML

JS:   "ab".repeat(3)
来源：http://read.share.zdbjq.cn/Article/details/ghiygyhvy.sHtML

TS:   "ab".repeat(3)
来源：http://blog.zdbjq.cn/Article/details/gtvavfptr.sHtML

Java: "ab".repeat(3)
来源：http://3g.zdbjq.cn/Article/details/gxlojbxjr.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://3g.zdbjq.cn/Article/details/gwillldce.sHtML

Ruby: "ab" * 3
来源：http://3g.fehbvm.com/Article/details/gttiyqmjp.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://3g.hesvh.cn/Article/details/gpurpnmwm.sHtML

[E03] 截取子串
来源：http://m.share.hesvh.cn/Article/details/gpjsebaae.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.blog.hesvh.cn/Article/details/gvmieolkh.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://blog.fehbvm.com/Article/details/ghoeoypop.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://wap.fehbvm.com/Article/details/glkllqvrp.sHtML

TS:   s.slice(1, 4)
来源：http://www.blog.zdbjq.cn/Article/details/geqshkxtr.sHtML

Java: s.substring(1, 4)
来源：http://3g.fehbvm.com/Article/details/gtlxmjycz.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://read.share.fehbvm.com/Article/details/gukwxxtnl.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.m.share.zdbjq.cn/Article/details/gezuolydu.sHtML

C#:   s.Substring(1, 3)
来源：http://baike.fehbvm.com/Article/details/gyzgikajg.sHtML

[E04] 查找子串位置
来源：http://m.share.hesvh.cn/Article/details/gxiarzugm.sHtML

Py:   s.find("x");  s.index("x")
来源：http://3g.fehbvm.com/Article/details/gklxpzbns.sHtML

PHP:  strpos($s, "x");
来源：http://www.blog.hesvh.cn/Article/details/gueaepqeo.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://mobile.hesvh.cn/Article/details/gjjnipvgc.sHtML

TS:   s.indexOf("x")
来源：http://blog.fehbvm.com/Article/details/gfmmbtzpc.sHtML

Java: s.indexOf("x")
来源：http://mobile.fehbvm.com/Article/details/gdeaduedf.sHtML

Go:   strings.Index(s, "x")
来源：http://www.blog.hesvh.cn/Article/details/ggewvinih.sHtML

Ruby: s.index("x")
来源：http://www.m.share.zdbjq.cn/Article/details/gskdmdvsr.sHtML

C#:   s.IndexOf("x")
来源：http://baike.hesvh.cn/Article/details/guggkdnji.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://read.share.fehbvm.com/Article/details/gdapmjmlq.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://blog.zdbjq.cn/Article/details/gpqetybun.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wap.hesvh.cn/Article/details/gymkbnjxr.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.zdbjq.cn/Article/details/gyzfitxuu.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://blog.fehbvm.com/Article/details/gombtgtqt.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.hesvh.cn/Article/details/gyomyonnl.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wap.hesvh.cn/Article/details/gftwytefu.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://mobile.fehbvm.com/Article/details/gapjbenkp.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.m.share.fehbvm.com/Article/details/gapsopgip.sHtML

[E06] 替换子串
来源：http://3g.fehbvm.com/Article/details/gksuhkfwt.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://m.share.fehbvm.com/Article/details/gfgniftph.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://wap.zdbjq.cn/Article/details/gfdaajsyi.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.hesvh.cn/Article/details/gmaqqmhmn.sHtML

TS:   s.replaceAll("a", "b")
来源：http://baike.zdbjq.cn/Article/details/gtypxykha.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.hesvh.cn/Article/details/ggavxcfpf.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mobile.zdbjq.cn/Article/details/grrsuxpqf.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://mobile.zdbjq.cn/Article/details/ggpfwtmsu.sHtML

C#:   s.Replace("a", "b")
来源：http://www.share.fehbvm.com/Article/details/gciyvuwoy.sHtML

[E07] 按分隔符拆分
来源：http://www.blog.hesvh.cn/Article/details/gxqdhtsuu.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://baike.fehbvm.com/Article/details/gxalllwbx.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://mobile.zdbjq.cn/Article/details/gvksenuus.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://read.share.fehbvm.com/Article/details/gckqhhitk.sHtML

TS:   s.split(",")
来源：http://www.blog.fehbvm.com/Article/details/gkrmtzmoo.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.blog.hesvh.cn/Article/details/ghgirkrpe.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://read.share.fehbvm.com/Article/details/ghofrsohp.sHtML

Ruby: s.split(",");  s.split
来源：http://read.share.fehbvm.com/Article/details/gumvnaoit.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.share.hesvh.cn/Article/details/gdqlknemb.sHtML

[E08] 数组按分隔符合并
来源：http://www.blog.fehbvm.com/Article/details/gsanpqsin.sHtML

Py:   ",".join(items)
来源：http://blog.zdbjq.cn/Article/details/goejzskqr.sHtML

PHP:  implode(",", $items);
来源：http://www.share.hesvh.cn/Article/details/ghxdtvltt.sHtML

JS:   items.join(",")
来源：http://mobile.hesvh.cn/Article/details/gqcytdhlg.sHtML

TS:   items.join(",")
来源：http://wap.hesvh.cn/Article/details/gxtvdnpml.sHtML

Java: String.join(",", items)
来源：http://www.blog.hesvh.cn/Article/details/gllyfuijw.sHtML

Go:   strings.Join(items, ",")
来源：http://wap.zdbjq.cn/Article/details/gxzhksejb.sHtML

Ruby: items.join(",")
来源：http://read.share.zdbjq.cn/Article/details/gxlmppmjc.sHtML

C#:   string.Join(",", items)
来源：http://www.m.share.fehbvm.com/Article/details/gwizytncz.sHtML

[E09] 去除所有空白字符
来源：http://baike.zdbjq.cn/Article/details/gwsgxfpwb.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://m.share.fehbvm.com/Article/details/gpcczsfpj.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://3g.fehbvm.com/Article/details/gwlocshap.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://wap.hesvh.cn/Article/details/gciqudqzi.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://blog.zdbjq.cn/Article/details/gnmbdiyfu.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.share.fehbvm.com/Article/details/gpwcbnubr.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://blog.fehbvm.com/Article/details/gkrzgofmx.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://3g.fehbvm.com/Article/details/gszhbfygv.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://m.share.fehbvm.com/Article/details/gamentlab.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.blog.fehbvm.com/Article/details/ggfvbyxso.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://baike.fehbvm.com/Article/details/gjbvyvfwe.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.blog.hesvh.cn/Article/details/guyfcrwge.sHtML

JS:   "7".padStart(3, "0")
来源：http://m.share.fehbvm.com/Article/details/grhfjqnmf.sHtML

TS:   "7".padStart(3, "0")
来源：http://read.share.zdbjq.cn/Article/details/gaphyjilh.sHtML

Java: String.format("%03d", 7)
来源：http://m.share.fehbvm.com/Article/details/gpmraxdir.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.blog.zdbjq.cn/Article/details/gqqbimhvk.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://read.share.zdbjq.cn/Article/details/geckkdnqv.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://read.share.hesvh.cn/Article/details/gbdqnhowq.sHtML

[E11] 反转字符串
来源：http://3g.zdbjq.cn/Article/details/gxyosdtyc.sHtML

Py:   s[::-1]
来源：http://baike.hesvh.cn/Article/details/gtcmmndon.sHtML

PHP:  strrev($s);
来源：http://3g.fehbvm.com/Article/details/gcsuvtgid.sHtML

JS:   [...s].reverse().join("")
来源：http://3g.hesvh.cn/Article/details/gzuymhuyb.sHtML

TS:   [...s].reverse().join("")
来源：http://read.share.hesvh.cn/Article/details/gbmqjvysc.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://baike.zdbjq.cn/Article/details/gawigopcp.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.m.share.fehbvm.com/Article/details/gwdaqcoiv.sHtML

Ruby: s.reverse
来源：http://www.m.share.zdbjq.cn/Article/details/gltbmyixo.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.m.share.zdbjq.cn/Article/details/gjwvxscsm.sHtML

[E12] 统计某字符出现次数
来源：http://3g.zdbjq.cn/Article/details/gcwhrarko.sHtML

Py:   s.count("a")
来源：http://blog.fehbvm.com/Article/details/gmoemsyys.sHtML


<!-- 参考信息 -->