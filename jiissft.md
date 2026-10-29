代发 wailian999

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.blog.hesvh.cn/Article/details/guaexgcbz.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.blog.hesvh.cn/Article/details/gxxnonfpl.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://baike.zdbjq.cn/Article/details/gdpupatfl.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://3g.zdbjq.cn/Article/details/giksikisf.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://mobile.zdbjq.cn/Article/details/gtdmdifwk.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.fehbvm.com/Article/details/gzgzkcmnh.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mobile.hesvh.cn/Article/details/giyjuvgue.sHtML

[D06] 数组长度
来源：http://m.share.zdbjq.cn/Article/details/gcgsazkec.sHtML

Py:   len(arr)
来源：http://www.share.hesvh.cn/Article/details/grvbsgyuz.sHtML

PHP:  count($arr);
来源：http://wap.hesvh.cn/Article/details/gnolbtgsc.sHtML

JS:   arr.length
来源：http://3g.zdbjq.cn/Article/details/ghdzstaep.sHtML

TS:   arr.length
来源：http://www.blog.zdbjq.cn/Article/details/grnrermsz.sHtML

Java: list.size();
来源：http://baike.zdbjq.cn/Article/details/glhhbzgit.sHtML

Go:   len(arr)
来源：http://www.share.zdbjq.cn/Article/details/grvxvhlhd.sHtML

Ruby: arr.length; arr.size
来源：http://www.m.share.zdbjq.cn/Article/details/gmsayumzo.sHtML

C#:   list.Count;
来源：http://www.m.share.zdbjq.cn/Article/details/gadbweebf.sHtML

[D07] 切片 / 取子数组
来源：http://read.share.zdbjq.cn/Article/details/glrsnogen.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://3g.zdbjq.cn/Article/details/galirqmzc.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://m.share.fehbvm.com/Article/details/gtlsxnjzn.sHtML

JS:   arr.slice(1, 4);
来源：http://www.share.fehbvm.com/Article/details/gwcascmoz.sHtML

TS:   arr.slice(1, 4);
来源：http://blog.zdbjq.cn/Article/details/gqyywueov.sHtML

Java: list.subList(1, 4);
来源：http://www.share.fehbvm.com/Article/details/giytbmndq.sHtML

Go:   arr[1:4]
来源：http://m.share.fehbvm.com/Article/details/gwsncsavr.sHtML

Ruby: arr[1, 3]
来源：http://3g.hesvh.cn/Article/details/gykgqhotq.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.blog.zdbjq.cn/Article/details/gmhrwgioj.sHtML

[D08] 合并两个数组
来源：http://baike.hesvh.cn/Article/details/gipdvwhaj.sHtML

Py:   a + b;  a.extend(b)
来源：http://m.share.hesvh.cn/Article/details/gfulmqioh.sHtML

PHP:  array_merge($a, $b);
来源：http://3g.zdbjq.cn/Article/details/gbrkdyfgl.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://baike.fehbvm.com/Article/details/gwfmormlk.sHtML

TS:   [...a, ...b];
来源：http://blog.hesvh.cn/Article/details/gizvpexma.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.share.zdbjq.cn/Article/details/ggootgjvw.sHtML

Go:   append(a, b...)
来源：http://m.share.zdbjq.cn/Article/details/gvhrhrtxx.sHtML

Ruby: a + b;  a.concat(b)
来源：http://baike.fehbvm.com/Article/details/gugftywlf.sHtML

C#:   a.Concat(b).ToList()
来源：http://baike.zdbjq.cn/Article/details/gjwvahkwl.sHtML

[D09] 排序（升序）
来源：http://3g.hesvh.cn/Article/details/ggiarvtoo.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.zdbjq.cn/Article/details/gaaanomzg.sHtML

PHP:  sort($arr);
来源：http://wap.hesvh.cn/Article/details/gamkihwwp.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://baike.fehbvm.com/Article/details/gxzhqacsc.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://wap.fehbvm.com/Article/details/gnnnojdcv.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.m.share.fehbvm.com/Article/details/gfjxitbco.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gumyvggjx.sHtML

Ruby: arr.sort
来源：http://www.m.share.zdbjq.cn/Article/details/gtxyrhgfs.sHtML

C#:   list.Sort();
来源：http://www.blog.hesvh.cn/Article/details/gsytmvcfr.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://3g.zdbjq.cn/Article/details/gwvmgwdft.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mobile.fehbvm.com/Article/details/gayygkkez.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.hesvh.cn/Article/details/gsdeqxrjv.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.fehbvm.com/Article/details/gtrbrsaiw.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.hesvh.cn/Article/details/gfbzekdrj.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://m.share.zdbjq.cn/Article/details/gffqwtayr.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.share.zdbjq.cn/Article/details/gotixmpvm.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mobile.fehbvm.com/Article/details/gqsvefjia.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://blog.hesvh.cn/Article/details/gwgyyxfgr.sHtML

[D11] 反转数组
来源：http://3g.hesvh.cn/Article/details/gbtzivjmx.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://wap.zdbjq.cn/Article/details/gfbcmhrxq.sHtML

PHP:  array_reverse($arr);
来源：http://m.share.hesvh.cn/Article/details/goiqutxft.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://m.share.zdbjq.cn/Article/details/gjxcmmfof.sHtML

TS:   [...arr].reverse();
来源：http://www.blog.zdbjq.cn/Article/details/glrlzqjps.sHtML

Java: Collections.reverse(list);
来源：http://www.share.hesvh.cn/Article/details/gpviooodd.sHtML

Go:   slices.Reverse(arr)
来源：http://3g.hesvh.cn/Article/details/gnxaigaza.sHtML

Ruby: arr.reverse
来源：http://blog.hesvh.cn/Article/details/geggczynk.sHtML

C#:   list.Reverse();
来源：http://m.share.hesvh.cn/Article/details/gqzfzyfgg.sHtML

[D12] 查找元素下标
来源：http://wap.fehbvm.com/Article/details/gqeqzkzpc.sHtML

Py:   arr.index(x);  x in arr
来源：http://blog.hesvh.cn/Article/details/gctmvmreq.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://read.share.hesvh.cn/Article/details/gwgqxaccm.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.hesvh.cn/Article/details/giqmexxki.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.zdbjq.cn/Article/details/gosnxjpuh.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://3g.fehbvm.com/Article/details/gzdksezur.sHtML

Go:   slices.Index(arr, x)
来源：http://blog.hesvh.cn/Article/details/gieusviig.sHtML

Ruby: arr.index(x)
来源：http://baike.fehbvm.com/Article/details/gdksjizou.sHtML

C#:   list.IndexOf(x);
来源：http://mobile.fehbvm.com/Article/details/grohkbalo.sHtML

[D13] 过滤（保留满足条件的）
来源：http://blog.fehbvm.com/Article/details/gdxapagda.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://mobile.fehbvm.com/Article/details/gxyziqbyr.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://m.share.zdbjq.cn/Article/details/gonjsjwcc.sHtML

JS:   arr.filter(x => x > 3)
来源：http://m.share.hesvh.cn/Article/details/gtczptofg.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.share.hesvh.cn/Article/details/gqcekfhkv.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.m.share.fehbvm.com/Article/details/giluznxbf.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.blog.hesvh.cn/Article/details/gtgdvbfvc.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://wap.hesvh.cn/Article/details/gsqtkrycx.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.share.zdbjq.cn/Article/details/geszuaihg.sHtML

[D14] 映射转换（每个元素变形）
来源：http://mobile.zdbjq.cn/Article/details/gdktkcrft.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://3g.hesvh.cn/Article/details/guhabjsvv.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://m.share.hesvh.cn/Article/details/ggqvmcwez.sHtML

JS:   arr.map(x => x * 2)
来源：http://blog.fehbvm.com/Article/details/gaqhuojof.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.share.zdbjq.cn/Article/details/glalcofmh.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://blog.fehbvm.com/Article/details/ghqxgrfzb.sHtML

Go:   // 手写循环
来源：http://baike.hesvh.cn/Article/details/gvlxppezt.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://baike.hesvh.cn/Article/details/gmjugtsqh.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://3g.zdbjq.cn/Article/details/gaayaowjx.sHtML

[D15] 去重
来源：http://www.share.fehbvm.com/Article/details/gmmghkqsx.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://wap.hesvh.cn/Article/details/growugvyg.sHtML

PHP:  array_unique($arr);
来源：http://baike.hesvh.cn/Article/details/gtodhmwnu.sHtML

JS:   [...new Set(arr)]
来源：http://wap.hesvh.cn/Article/details/gijdnyggp.sHtML

TS:   [...new Set(arr)]
来源：http://blog.hesvh.cn/Article/details/gxtloesal.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.m.share.fehbvm.com/Article/details/gfeouryld.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://baike.hesvh.cn/Article/details/giiqzklqh.sHtML

Ruby: arr.uniq
来源：http://mobile.zdbjq.cn/Article/details/gqecmpitj.sHtML

C#:   list.Distinct().ToList()
来源：http://mobile.zdbjq.cn/Article/details/gkhxfwtwg.sHtML

[D16] 求和与平均值
来源：http://wap.zdbjq.cn/Article/details/ggxdlennp.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.blog.fehbvm.com/Article/details/grsjfwdov.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://blog.fehbvm.com/Article/details/gloheporr.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.hesvh.cn/Article/details/gnjzosicw.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.fehbvm.com/Article/details/gzulermwb.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://blog.zdbjq.cn/Article/details/grewapybt.sHtML

Go:   // 手写循环累加
来源：http://www.share.fehbvm.com/Article/details/gniskotlr.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://read.share.hesvh.cn/Article/details/gnfdyjnas.sHtML

C#:   list.Sum();  list.Average()
来源：http://mobile.zdbjq.cn/Article/details/gqlhkaxnt.sHtML

[D17] 最大值与最小值
来源：http://mobile.fehbvm.com/Article/details/guckeiubp.sHtML

Py:   max(arr);  min(arr)
来源：http://www.share.fehbvm.com/Article/details/gscplvrmb.sHtML

PHP:  max($arr);  min($arr);
来源：http://baike.fehbvm.com/Article/details/gwbjiwvou.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://3g.fehbvm.com/Article/details/gdikcqvgi.sHtML

TS:   Math.max(...arr);
来源：http://3g.hesvh.cn/Article/details/goakjuqcg.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://read.share.hesvh.cn/Article/details/gdgymdlmm.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wap.fehbvm.com/Article/details/gyxovovpw.sHtML

Ruby: arr.max;  arr.min
来源：http://baike.hesvh.cn/Article/details/gllqqzhha.sHtML

C#:   list.Max();  list.Min()
来源：http://blog.fehbvm.com/Article/details/gsahijqfx.sHtML

[D18] 扁平化嵌套数组
来源：http://www.m.share.zdbjq.cn/Article/details/gxnfqiitv.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mobile.zdbjq.cn/Article/details/gajrzexrx.sHtML

PHP:  array_merge(...$nested);
来源：http://blog.hesvh.cn/Article/details/gxobyskwj.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://blog.hesvh.cn/Article/details/glymumbhm.sHtML

TS:   nested.flat();
来源：http://baike.hesvh.cn/Article/details/gllwtrpoo.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://read.share.fehbvm.com/Article/details/gzwttszsm.sHtML

Go:   // 手写双层循环
来源：http://www.share.zdbjq.cn/Article/details/gtsjqfzwu.sHtML

Ruby: nested.flatten
来源：http://read.share.fehbvm.com/Article/details/gnethumep.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://read.share.fehbvm.com/Article/details/gsykflgkq.sHtML

[D19] 按字段分组
来源：http://blog.hesvh.cn/Article/details/gfdojaayp.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wap.zdbjq.cn/Article/details/gtbeiuosa.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://m.share.hesvh.cn/Article/details/gkicwnubf.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.blog.fehbvm.com/Article/details/gyyrkbblx.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://wap.zdbjq.cn/Article/details/gjwjttobc.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://blog.fehbvm.com/Article/details/gxfsgkire.sHtML

Go:   // 手写 map[string][]T
来源：http://www.blog.fehbvm.com/Article/details/gvpoipara.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://baike.zdbjq.cn/Article/details/gkhapgztd.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://m.share.zdbjq.cn/Article/details/gboetchsj.sHtML

[D20] 统计每个元素出现次数
来源：http://www.blog.fehbvm.com/Article/details/gyjyqcsdd.sHtML

Py:   Counter(arr)
来源：http://wap.hesvh.cn/Article/details/gazvczdal.sHtML

PHP:  array_count_values($arr);
来源：http://wap.zdbjq.cn/Article/details/gzmcdqiye.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.fehbvm.com/Article/details/gkezxfkgz.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.fehbvm.com/Article/details/gvzrdwoff.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://blog.zdbjq.cn/Article/details/gdaevwshz.sHtML

Go:   // 手写 map[T]int
来源：http://m.share.zdbjq.cn/Article/details/ggaijstym.sHtML

Ruby: arr.tally
来源：http://mobile.zdbjq.cn/Article/details/gtvvhcpwa.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://blog.fehbvm.com/Article/details/gnkpdvhoh.sHtML

[D21] 判断是否包含某元素
来源：http://www.blog.fehbvm.com/Article/details/gjbdnaray.sHtML

Py:   x in arr
来源：http://baike.fehbvm.com/Article/details/gqpvnukix.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.share.hesvh.cn/Article/details/gcvpmjyeh.sHtML

JS:   arr.includes(x)
来源：http://www.m.share.fehbvm.com/Article/details/gkjzyylgj.sHtML

TS:   arr.includes(x)
来源：http://mobile.zdbjq.cn/Article/details/gmmatftzl.sHtML

Java: list.contains(x)
来源：http://www.blog.fehbvm.com/Article/details/glozojxpt.sHtML

Go:   slices.Contains(arr, x)
来源：http://wap.hesvh.cn/Article/details/gyuvihnlc.sHtML

Ruby: arr.include?(x)
来源：http://wap.zdbjq.cn/Article/details/gudwiqcej.sHtML

C#:   list.Contains(x)
来源：http://baike.hesvh.cn/Article/details/gfipyyunl.sHtML

[D22] 复制数组（避免共享引用）
来源：http://blog.hesvh.cn/Article/details/gibrifwxo.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gsqcmpgvk.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.m.share.fehbvm.com/Article/details/gpuflehsi.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://read.share.hesvh.cn/Article/details/gglczyfrj.sHtML

TS:   [...arr];
来源：http://m.share.fehbvm.com/Article/details/gitjtshom.sHtML

Java: new ArrayList<>(list);
来源：http://mobile.hesvh.cn/Article/details/gfqmtdoza.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://m.share.zdbjq.cn/Article/details/gcdqsysmh.sHtML

Ruby: arr.dup;  arr.clone
来源：http://3g.fehbvm.com/Article/details/gorpbplor.sHtML

C#:   new List<int>(list);
来源：http://wap.hesvh.cn/Article/details/gveqmkusz.sHtML

[D23] reduce 累积计算
来源：http://baike.zdbjq.cn/Article/details/ggkogikyz.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wap.zdbjq.cn/Article/details/gznoewrfm.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://baike.hesvh.cn/Article/details/gzmherthz.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.zdbjq.cn/Article/details/gbgihqnoy.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.zdbjq.cn/Article/details/gmwsghbzq.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://mobile.hesvh.cn/Article/details/gzqvgzrqs.sHtML

Go:   // 手写循环
来源：http://wap.fehbvm.com/Article/details/gjdufaqec.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://blog.fehbvm.com/Article/details/gpinstukt.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.blog.hesvh.cn/Article/details/gaggbyzbj.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.share.zdbjq.cn/Article/details/gyftjrxuz.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mobile.zdbjq.cn/Article/details/gomyjtfgg.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://wap.zdbjq.cn/Article/details/gjbowhdgx.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wap.zdbjq.cn/Article/details/gkeasxjqp.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.blog.zdbjq.cn/Article/details/grctjpqld.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://mobile.zdbjq.cn/Article/details/gqtnlyhgo.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://m.share.fehbvm.com/Article/details/gyafqhcox.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://mobile.zdbjq.cn/Article/details/gsxjqcvcy.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://3g.zdbjq.cn/Article/details/gpmgmgafm.sHtML

[D25] Set 集合去重与交并差
来源：http://read.share.fehbvm.com/Article/details/glooyebpb.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wap.hesvh.cn/Article/details/grtvgutyw.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://read.share.hesvh.cn/Article/details/gttriqgcd.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://m.share.zdbjq.cn/Article/details/gjytpwjpi.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mobile.fehbvm.com/Article/details/givebykua.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://3g.hesvh.cn/Article/details/gbwrzgwkw.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.share.zdbjq.cn/Article/details/geasjsxau.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wap.hesvh.cn/Article/details/gkwpttunx.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://baike.hesvh.cn/Article/details/gsxjmjefo.sHtML

[D26] 数组转字符串
来源：http://www.share.hesvh.cn/Article/details/ggnrgjote.sHtML

Py:   ", ".join(map(str, arr))
来源：http://3g.fehbvm.com/Article/details/gmjlgfcmz.sHtML

PHP:  implode(", ", $arr);
来源：http://www.share.zdbjq.cn/Article/details/ggyxekxwg.sHtML

JS:   arr.join(", ")
来源：http://mobile.zdbjq.cn/Article/details/gfvblrcgl.sHtML

TS:   arr.join(", ")
来源：http://www.share.fehbvm.com/Article/details/genbubvzq.sHtML

Java: String.join(", ", list)
来源：http://www.m.share.fehbvm.com/Article/details/gqbbanlrl.sHtML

Go:   strings.Join(strs, ", ")
来源：http://blog.zdbjq.cn/Article/details/gpdvlpmnx.sHtML

Ruby: arr.join(", ")
来源：http://blog.zdbjq.cn/Article/details/gyqkqzaqs.sHtML

C#:   string.Join(", ", list)
来源：http://read.share.hesvh.cn/Article/details/gpwnicwli.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gubfenacp.sHtML

E. 字符串处理
来源：http://blog.zdbjq.cn/Article/details/gulfsaxxf.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gxtmjtkmp.sHtML

[E01] 拼接字符串
来源：http://blog.hesvh.cn/Article/details/gfdzkwtsf.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://blog.fehbvm.com/Article/details/gyepkxepy.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://baike.fehbvm.com/Article/details/gyszqiwmq.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.zdbjq.cn/Article/details/ggjmsgacv.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.hesvh.cn/Article/details/ghpxzbzyv.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://m.share.zdbjq.cn/Article/details/gkawtovyf.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://m.share.fehbvm.com/Article/details/gtitacjpn.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wap.hesvh.cn/Article/details/gqsnjlbjt.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://read.share.fehbvm.com/Article/details/gpwsztito.sHtML

[E02] 重复字符串
来源：http://3g.zdbjq.cn/Article/details/gbihartmm.sHtML

Py:   "ab" * 3
来源：http://blog.hesvh.cn/Article/details/gvsxsttxy.sHtML

PHP:  str_repeat("ab", 3);
来源：http://baike.fehbvm.com/Article/details/gddmqhihi.sHtML

JS:   "ab".repeat(3)
来源：http://3g.hesvh.cn/Article/details/gjvucmsgz.sHtML

TS:   "ab".repeat(3)
来源：http://m.share.zdbjq.cn/Article/details/gpcwnszuq.sHtML

Java: "ab".repeat(3)
来源：http://wap.zdbjq.cn/Article/details/giqvnbwzl.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://3g.fehbvm.com/Article/details/gztuqhznp.sHtML

Ruby: "ab" * 3
来源：http://baike.hesvh.cn/Article/details/gpzqxiuqt.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://read.share.zdbjq.cn/Article/details/gojcawrpu.sHtML

[E03] 截取子串
来源：http://baike.hesvh.cn/Article/details/gtmqcegmd.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wap.hesvh.cn/Article/details/grelhdpjg.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.share.hesvh.cn/Article/details/gdhhgnkca.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://m.share.hesvh.cn/Article/details/goxptbqqe.sHtML

TS:   s.slice(1, 4)
来源：http://www.m.share.fehbvm.com/Article/details/gisihmjyg.sHtML

Java: s.substring(1, 4)
来源：http://read.share.hesvh.cn/Article/details/gxzkdwmuv.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://m.share.hesvh.cn/Article/details/gfouhvtic.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://3g.fehbvm.com/Article/details/ggpdzuxmv.sHtML

C#:   s.Substring(1, 3)
来源：http://wap.zdbjq.cn/Article/details/ghlscgkys.sHtML

[E04] 查找子串位置
来源：http://blog.zdbjq.cn/Article/details/gkjrmyxdt.sHtML

Py:   s.find("x");  s.index("x")
来源：http://baike.zdbjq.cn/Article/details/glulisjzw.sHtML

PHP:  strpos($s, "x");
来源：http://wap.zdbjq.cn/Article/details/gxhelrhwn.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://blog.fehbvm.com/Article/details/gpqfqmreb.sHtML

TS:   s.indexOf("x")
来源：http://read.share.fehbvm.com/Article/details/gcbpgqnvs.sHtML

Java: s.indexOf("x")
来源：http://blog.fehbvm.com/Article/details/gqimpbhau.sHtML

Go:   strings.Index(s, "x")
来源：http://m.share.hesvh.cn/Article/details/gguzuhsjz.sHtML

Ruby: s.index("x")
来源：http://www.m.share.zdbjq.cn/Article/details/gtyfrmnxi.sHtML

C#:   s.IndexOf("x")
来源：http://www.blog.fehbvm.com/Article/details/gbztnczkg.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://read.share.zdbjq.cn/Article/details/glfpvuxhe.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://baike.zdbjq.cn/Article/details/gkincbbmb.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.blog.fehbvm.com/Article/details/gtjiuupln.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.fehbvm.com/Article/details/gbwspmybm.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://baike.fehbvm.com/Article/details/grcyyrmgd.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.hesvh.cn/Article/details/gcjxeorfz.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://baike.fehbvm.com/Article/details/gywxkbvrl.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://mobile.hesvh.cn/Article/details/gwcrsmmiz.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://wap.hesvh.cn/Article/details/gwrarnwed.sHtML

[E06] 替换子串
来源：http://baike.zdbjq.cn/Article/details/gaeposbmr.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.m.share.fehbvm.com/Article/details/gkkuvdupj.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://mobile.fehbvm.com/Article/details/gjfmamtff.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.fehbvm.com/Article/details/glgtqxppv.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/gxkikpzqh.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/gqhycpufc.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mobile.fehbvm.com/Article/details/gcvmjizsx.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://wap.zdbjq.cn/Article/details/ghaxhyngh.sHtML

C#:   s.Replace("a", "b")
来源：http://baike.zdbjq.cn/Article/details/glxeantrq.sHtML

[E07] 按分隔符拆分
来源：http://3g.hesvh.cn/Article/details/gfnzvgbis.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://m.share.zdbjq.cn/Article/details/gozvfzcrb.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.m.share.zdbjq.cn/Article/details/gjzaeumdm.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://m.share.zdbjq.cn/Article/details/giohkqyae.sHtML

TS:   s.split(",")
来源：http://3g.fehbvm.com/Article/details/gkyzsatvk.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.blog.zdbjq.cn/Article/details/gztqhanws.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.blog.zdbjq.cn/Article/details/ghecagxlq.sHtML

Ruby: s.split(",");  s.split
来源：http://www.share.hesvh.cn/Article/details/gonouzrqv.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.blog.zdbjq.cn/Article/details/ggmnnnopj.sHtML

[E08] 数组按分隔符合并
来源：http://3g.hesvh.cn/Article/details/gzrfgoknt.sHtML

Py:   ",".join(items)
来源：http://baike.hesvh.cn/Article/details/gqfvzkcex.sHtML

PHP:  implode(",", $items);
来源：http://m.share.fehbvm.com/Article/details/ghnjwkplo.sHtML

JS:   items.join(",")
来源：http://blog.zdbjq.cn/Article/details/goipeslmu.sHtML

TS:   items.join(",")
来源：http://www.share.zdbjq.cn/Article/details/guopstjoj.sHtML

Java: String.join(",", items)
来源：http://wap.zdbjq.cn/Article/details/guyhfoyuz.sHtML

Go:   strings.Join(items, ",")
来源：http://www.m.share.fehbvm.com/Article/details/gauztllxn.sHtML

Ruby: items.join(",")
来源：http://m.share.zdbjq.cn/Article/details/gyflbneee.sHtML

C#:   string.Join(",", items)
来源：http://read.share.fehbvm.com/Article/details/geqtdufhj.sHtML

[E09] 去除所有空白字符
来源：http://mobile.hesvh.cn/Article/details/gkvxmgjsx.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://m.share.zdbjq.cn/Article/details/grexszpns.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://3g.fehbvm.com/Article/details/ghfyllgyl.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.m.share.hesvh.cn/Article/details/gloxroyal.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://read.share.zdbjq.cn/Article/details/gfpjyidpk.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://wap.fehbvm.com/Article/details/glnruqqkb.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.blog.zdbjq.cn/Article/details/gdebjktjc.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://mobile.zdbjq.cn/Article/details/gqlajblev.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://m.share.zdbjq.cn/Article/details/gffsdplqq.sHtML

[E10] 左侧补零 / 定长填充
来源：http://baike.fehbvm.com/Article/details/gkzeullom.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://read.share.zdbjq.cn/Article/details/gjsfnfzjy.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://read.share.hesvh.cn/Article/details/grjomviwz.sHtML

JS:   "7".padStart(3, "0")
来源：http://blog.fehbvm.com/Article/details/gwogubnuw.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.blog.hesvh.cn/Article/details/glepdikgl.sHtML

Java: String.format("%03d", 7)
来源：http://www.blog.fehbvm.com/Article/details/gevdxjdmh.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.m.share.fehbvm.com/Article/details/gkqhrrezc.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://3g.zdbjq.cn/Article/details/gfktpyuhv.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://m.share.hesvh.cn/Article/details/gfovrhftw.sHtML

[E11] 反转字符串
来源：http://3g.fehbvm.com/Article/details/gvjnrmzwr.sHtML

Py:   s[::-1]
来源：http://www.share.zdbjq.cn/Article/details/gvfaughdd.sHtML

PHP:  strrev($s);
来源：http://baike.zdbjq.cn/Article/details/gqnlkewmo.sHtML

JS:   [...s].reverse().join("")
来源：http://baike.fehbvm.com/Article/details/ghodwlkvs.sHtML

TS:   [...s].reverse().join("")
来源：http://wap.zdbjq.cn/Article/details/gfxocznqh.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.m.share.hesvh.cn/Article/details/gqyidpbos.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.m.share.zdbjq.cn/Article/details/gjlsgdtma.sHtML

Ruby: s.reverse
来源：http://www.m.share.fehbvm.com/Article/details/geqnsfcdh.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.share.hesvh.cn/Article/details/guekzvylt.sHtML

[E12] 统计某字符出现次数
来源：http://www.m.share.fehbvm.com/Article/details/gtkichnix.sHtML

Py:   s.count("a")
来源：http://mobile.zdbjq.cn/Article/details/gwtqvkfcg.sHtML


<!-- 参考信息 -->