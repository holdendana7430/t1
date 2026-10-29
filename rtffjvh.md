代发 wailian999

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://read.share.fehbvm.com/Article/details/gnfxgzyvg.sHtML

TS:   arr.splice(0, 1);
来源：http://3g.fehbvm.com/Article/details/gznxuevru.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://baike.hesvh.cn/Article/details/gkuqaebpx.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.share.zdbjq.cn/Article/details/guckiqgld.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://blog.hesvh.cn/Article/details/ghikaebxi.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.share.zdbjq.cn/Article/details/gfdkkydac.sHtML

[D05] 访问与修改元素
来源：http://www.share.hesvh.cn/Article/details/gzuurzjzk.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.fehbvm.com/Article/details/ggssseaoa.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wap.fehbvm.com/Article/details/gqjliwnmo.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.blog.hesvh.cn/Article/details/gqmrsfjyh.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://3g.fehbvm.com/Article/details/gjgdfvoak.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.share.hesvh.cn/Article/details/gmsvgscyu.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://m.share.fehbvm.com/Article/details/gjxinjaph.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.fehbvm.com/Article/details/gvsyentug.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://blog.zdbjq.cn/Article/details/ghzjrbdgy.sHtML

[D06] 数组长度
来源：http://3g.fehbvm.com/Article/details/gpvgmfxtt.sHtML

Py:   len(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gkmdswkux.sHtML

PHP:  count($arr);
来源：http://3g.zdbjq.cn/Article/details/gcngiwwud.sHtML

JS:   arr.length
来源：http://mobile.zdbjq.cn/Article/details/gaafxwtna.sHtML

TS:   arr.length
来源：http://blog.zdbjq.cn/Article/details/gfkrnmojd.sHtML

Java: list.size();
来源：http://baike.hesvh.cn/Article/details/gbwvfowty.sHtML

Go:   len(arr)
来源：http://www.m.share.fehbvm.com/Article/details/ghztigayp.sHtML

Ruby: arr.length; arr.size
来源：http://www.m.share.hesvh.cn/Article/details/gzcviiitu.sHtML

C#:   list.Count;
来源：http://www.m.share.fehbvm.com/Article/details/gvfputxmr.sHtML

[D07] 切片 / 取子数组
来源：http://blog.fehbvm.com/Article/details/gewtgqrnz.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://3g.fehbvm.com/Article/details/ghqeqxdtt.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.blog.fehbvm.com/Article/details/gclqtsvam.sHtML

JS:   arr.slice(1, 4);
来源：http://www.share.hesvh.cn/Article/details/gzpnfvqst.sHtML

TS:   arr.slice(1, 4);
来源：http://www.share.hesvh.cn/Article/details/gfglveouv.sHtML

Java: list.subList(1, 4);
来源：http://mobile.zdbjq.cn/Article/details/gewhwivzo.sHtML

Go:   arr[1:4]
来源：http://blog.fehbvm.com/Article/details/gtqwzjmpx.sHtML

Ruby: arr[1, 3]
来源：http://read.share.zdbjq.cn/Article/details/giligqxdp.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.blog.hesvh.cn/Article/details/gegjyacob.sHtML

[D08] 合并两个数组
来源：http://read.share.zdbjq.cn/Article/details/gamondqtd.sHtML

Py:   a + b;  a.extend(b)
来源：http://read.share.zdbjq.cn/Article/details/ghalfwgwg.sHtML

PHP:  array_merge($a, $b);
来源：http://www.m.share.zdbjq.cn/Article/details/gqmjtivme.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://baike.hesvh.cn/Article/details/ggbfypysu.sHtML

TS:   [...a, ...b];
来源：http://www.share.fehbvm.com/Article/details/gykzxtsqu.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://3g.zdbjq.cn/Article/details/gdprtupna.sHtML

Go:   append(a, b...)
来源：http://wap.zdbjq.cn/Article/details/ggeqvsugz.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.blog.fehbvm.com/Article/details/gpxvgrbcx.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.share.fehbvm.com/Article/details/gbgojnqlc.sHtML

[D09] 排序（升序）
来源：http://wap.zdbjq.cn/Article/details/gvivgrsuq.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.hesvh.cn/Article/details/ghfpyefob.sHtML

PHP:  sort($arr);
来源：http://blog.hesvh.cn/Article/details/gxrascuhx.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.m.share.fehbvm.com/Article/details/gjznuvrno.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.share.fehbvm.com/Article/details/giabnzrwg.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.share.zdbjq.cn/Article/details/gkvzkzsps.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gbheqaypr.sHtML

Ruby: arr.sort
来源：http://m.share.zdbjq.cn/Article/details/gfcvarwen.sHtML

C#:   list.Sort();
来源：http://baike.fehbvm.com/Article/details/gvcwgykks.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://3g.zdbjq.cn/Article/details/gacmnofor.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.blog.hesvh.cn/Article/details/gnbxihvqf.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.zdbjq.cn/Article/details/gijazwdmk.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.hesvh.cn/Article/details/gxpyvukco.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.hesvh.cn/Article/details/gzqehgpmo.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://m.share.zdbjq.cn/Article/details/gevlaccow.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.share.hesvh.cn/Article/details/gagkipbrc.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.share.fehbvm.com/Article/details/gitxpmhdk.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://read.share.hesvh.cn/Article/details/gsmodsdwy.sHtML

[D11] 反转数组
来源：http://m.share.fehbvm.com/Article/details/gdkitgvty.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.share.zdbjq.cn/Article/details/gbnaxeudw.sHtML

PHP:  array_reverse($arr);
来源：http://baike.fehbvm.com/Article/details/gaeqhdgbg.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.m.share.hesvh.cn/Article/details/gwlwdecxn.sHtML

TS:   [...arr].reverse();
来源：http://www.blog.zdbjq.cn/Article/details/gtfaoczai.sHtML

Java: Collections.reverse(list);
来源：http://mobile.hesvh.cn/Article/details/gfviyjour.sHtML

Go:   slices.Reverse(arr)
来源：http://blog.hesvh.cn/Article/details/gfuimlrci.sHtML

Ruby: arr.reverse
来源：http://baike.fehbvm.com/Article/details/gwdfzeejb.sHtML

C#:   list.Reverse();
来源：http://m.share.hesvh.cn/Article/details/gevarxsqb.sHtML

[D12] 查找元素下标
来源：http://wap.fehbvm.com/Article/details/gljxsyjjt.sHtML

Py:   arr.index(x);  x in arr
来源：http://blog.hesvh.cn/Article/details/gdxtlvgoi.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://blog.hesvh.cn/Article/details/gixrnmuph.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.hesvh.cn/Article/details/gxnezvsji.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.fehbvm.com/Article/details/goeicktli.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.blog.hesvh.cn/Article/details/gtxtwzozp.sHtML

Go:   slices.Index(arr, x)
来源：http://3g.zdbjq.cn/Article/details/gteyeiahd.sHtML

Ruby: arr.index(x)
来源：http://wap.fehbvm.com/Article/details/gjbwhcclz.sHtML

C#:   list.IndexOf(x);
来源：http://www.m.share.fehbvm.com/Article/details/gimmkihkq.sHtML

[D13] 过滤（保留满足条件的）
来源：http://read.share.zdbjq.cn/Article/details/gcuipiari.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://wap.fehbvm.com/Article/details/grhrwojem.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://read.share.zdbjq.cn/Article/details/gxgndbtxk.sHtML

JS:   arr.filter(x => x > 3)
来源：http://wap.fehbvm.com/Article/details/gfyrxbggc.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.share.hesvh.cn/Article/details/gnmoaynku.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.blog.hesvh.cn/Article/details/grfnbjert.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.share.hesvh.cn/Article/details/grpdjejte.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://read.share.hesvh.cn/Article/details/gjwccwmnx.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://baike.zdbjq.cn/Article/details/gzkhvybeb.sHtML

[D14] 映射转换（每个元素变形）
来源：http://m.share.hesvh.cn/Article/details/gxcnrigmu.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mobile.zdbjq.cn/Article/details/gdxeoqfhf.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://m.share.hesvh.cn/Article/details/guvlvthfc.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.blog.fehbvm.com/Article/details/gnhqexhir.sHtML

TS:   arr.map(x => x * 2)
来源：http://mobile.hesvh.cn/Article/details/gkgdgwfhq.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.blog.fehbvm.com/Article/details/gcqtztiey.sHtML

Go:   // 手写循环
来源：http://blog.zdbjq.cn/Article/details/gjsqmpetj.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://wap.zdbjq.cn/Article/details/grsixoqxb.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.share.hesvh.cn/Article/details/gwkczrock.sHtML

[D15] 去重
来源：http://m.share.hesvh.cn/Article/details/gcuvgtaaw.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://blog.hesvh.cn/Article/details/gdpriwbtl.sHtML

PHP:  array_unique($arr);
来源：http://mobile.fehbvm.com/Article/details/gnhcnossf.sHtML

JS:   [...new Set(arr)]
来源：http://www.share.zdbjq.cn/Article/details/gubmjgyew.sHtML

TS:   [...new Set(arr)]
来源：http://read.share.fehbvm.com/Article/details/gxwzzbuma.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://m.share.hesvh.cn/Article/details/ggkfkduvd.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://baike.hesvh.cn/Article/details/gclxppxnk.sHtML

Ruby: arr.uniq
来源：http://m.share.fehbvm.com/Article/details/gzzkamyyo.sHtML

C#:   list.Distinct().ToList()
来源：http://baike.fehbvm.com/Article/details/gmtyknhul.sHtML

[D16] 求和与平均值
来源：http://www.m.share.hesvh.cn/Article/details/gnifyhdcv.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://3g.zdbjq.cn/Article/details/gzwxkkhep.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mobile.fehbvm.com/Article/details/gmroapqsa.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.zdbjq.cn/Article/details/gtfwdtcas.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.zdbjq.cn/Article/details/gyfdskfrq.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.blog.hesvh.cn/Article/details/gmntxlnkj.sHtML

Go:   // 手写循环累加
来源：http://baike.fehbvm.com/Article/details/gaerqubpu.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.share.hesvh.cn/Article/details/glucljpus.sHtML

C#:   list.Sum();  list.Average()
来源：http://wap.fehbvm.com/Article/details/gowsltnxx.sHtML

[D17] 最大值与最小值
来源：http://read.share.zdbjq.cn/Article/details/gyejlvbiy.sHtML

Py:   max(arr);  min(arr)
来源：http://mobile.hesvh.cn/Article/details/gkcrkmoke.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.blog.fehbvm.com/Article/details/grssbluwn.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.m.share.hesvh.cn/Article/details/gwbbujfno.sHtML

TS:   Math.max(...arr);
来源：http://read.share.zdbjq.cn/Article/details/ggbldoova.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://wap.hesvh.cn/Article/details/giwjbquxw.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wap.zdbjq.cn/Article/details/gdskvmqzn.sHtML

Ruby: arr.max;  arr.min
来源：http://www.blog.zdbjq.cn/Article/details/gmrppkgmd.sHtML

C#:   list.Max();  list.Min()
来源：http://www.blog.fehbvm.com/Article/details/gemsruvgr.sHtML

[D18] 扁平化嵌套数组
来源：http://3g.hesvh.cn/Article/details/gepuepeba.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.share.fehbvm.com/Article/details/gunncepqe.sHtML

PHP:  array_merge(...$nested);
来源：http://read.share.hesvh.cn/Article/details/gnqasfbcu.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mobile.fehbvm.com/Article/details/gcchvdrez.sHtML

TS:   nested.flat();
来源：http://read.share.fehbvm.com/Article/details/gwptrjpur.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://3g.fehbvm.com/Article/details/gfebzdvpf.sHtML

Go:   // 手写双层循环
来源：http://www.share.hesvh.cn/Article/details/gpeemyjoe.sHtML

Ruby: nested.flatten
来源：http://www.blog.zdbjq.cn/Article/details/ggglltlpf.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://read.share.fehbvm.com/Article/details/gllyruapu.sHtML

[D19] 按字段分组
来源：http://www.share.hesvh.cn/Article/details/gsawpcbjm.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wap.hesvh.cn/Article/details/gdtwdxtof.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wap.hesvh.cn/Article/details/ghhytizik.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://m.share.zdbjq.cn/Article/details/ghukdhroa.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://read.share.zdbjq.cn/Article/details/gmluhiwqk.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://baike.hesvh.cn/Article/details/gkajqblhn.sHtML

Go:   // 手写 map[string][]T
来源：http://m.share.zdbjq.cn/Article/details/gywquhoqb.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.blog.zdbjq.cn/Article/details/geycewfxq.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://blog.zdbjq.cn/Article/details/glzipuxpc.sHtML

[D20] 统计每个元素出现次数
来源：http://m.share.zdbjq.cn/Article/details/ggzlquwak.sHtML

Py:   Counter(arr)
来源：http://www.blog.fehbvm.com/Article/details/gdnnbqkno.sHtML

PHP:  array_count_values($arr);
来源：http://wap.hesvh.cn/Article/details/gepqwanih.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.fehbvm.com/Article/details/gkkctsdks.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.zdbjq.cn/Article/details/goatxyleq.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://m.share.zdbjq.cn/Article/details/gdinahxgh.sHtML

Go:   // 手写 map[T]int
来源：http://www.blog.fehbvm.com/Article/details/gaqypsnaj.sHtML

Ruby: arr.tally
来源：http://www.share.fehbvm.com/Article/details/gbtmkjowz.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://blog.fehbvm.com/Article/details/gogqqtcfb.sHtML

[D21] 判断是否包含某元素
来源：http://m.share.fehbvm.com/Article/details/gipayxeqt.sHtML

Py:   x in arr
来源：http://m.share.fehbvm.com/Article/details/gfcwzeixy.sHtML

PHP:  in_array($x, $arr, true);
来源：http://wap.hesvh.cn/Article/details/gufkcnomh.sHtML

JS:   arr.includes(x)
来源：http://baike.fehbvm.com/Article/details/gywakmrnc.sHtML

TS:   arr.includes(x)
来源：http://baike.zdbjq.cn/Article/details/guxoizmxu.sHtML

Java: list.contains(x)
来源：http://mobile.zdbjq.cn/Article/details/geofduanr.sHtML

Go:   slices.Contains(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/gufcnrtsq.sHtML

Ruby: arr.include?(x)
来源：http://read.share.fehbvm.com/Article/details/gplgqsgxd.sHtML

C#:   list.Contains(x)
来源：http://3g.fehbvm.com/Article/details/gzvwggfni.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.blog.hesvh.cn/Article/details/gimppshka.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.share.fehbvm.com/Article/details/gxpsjpaee.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://blog.hesvh.cn/Article/details/gtlynafck.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://m.share.fehbvm.com/Article/details/gcttouixd.sHtML

TS:   [...arr];
来源：http://www.blog.fehbvm.com/Article/details/glrafrhdb.sHtML

Java: new ArrayList<>(list);
来源：http://www.m.share.zdbjq.cn/Article/details/gutbdprrx.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://read.share.hesvh.cn/Article/details/geiwaesjw.sHtML

Ruby: arr.dup;  arr.clone
来源：http://baike.hesvh.cn/Article/details/gawpdlntw.sHtML

C#:   new List<int>(list);
来源：http://www.m.share.fehbvm.com/Article/details/gzenavhzh.sHtML

[D23] reduce 累积计算
来源：http://read.share.hesvh.cn/Article/details/grjdxbmng.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://mobile.zdbjq.cn/Article/details/gtxiovaza.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://m.share.hesvh.cn/Article/details/gdeliuncs.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.fehbvm.com/Article/details/gyyrhssen.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.fehbvm.com/Article/details/gqiajbcoy.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.blog.fehbvm.com/Article/details/gjbtfnwiv.sHtML

Go:   // 手写循环
来源：http://wap.hesvh.cn/Article/details/gpkbgkaua.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mobile.hesvh.cn/Article/details/gykgyggax.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://baike.hesvh.cn/Article/details/gczbwxixt.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.share.hesvh.cn/Article/details/gmnhqgoqi.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mobile.zdbjq.cn/Article/details/gbwhdwjun.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://blog.fehbvm.com/Article/details/gvvotaqnx.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://read.share.fehbvm.com/Article/details/guvfulzeb.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.share.fehbvm.com/Article/details/gygbpsynw.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://read.share.zdbjq.cn/Article/details/gyvswluse.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://m.share.hesvh.cn/Article/details/gfpsntgrx.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.blog.zdbjq.cn/Article/details/gjyuailxs.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mobile.hesvh.cn/Article/details/gcssibeyv.sHtML

[D25] Set 集合去重与交并差
来源：http://www.blog.fehbvm.com/Article/details/gxesexabx.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://read.share.hesvh.cn/Article/details/gzlmlkzeb.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://m.share.zdbjq.cn/Article/details/gjrjdqvae.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.m.share.fehbvm.com/Article/details/gyshbbuzc.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://baike.zdbjq.cn/Article/details/ghtciwtom.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://mobile.zdbjq.cn/Article/details/gobdnfddx.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://mobile.hesvh.cn/Article/details/giowtaowf.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://blog.fehbvm.com/Article/details/gyfgefqlw.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://read.share.zdbjq.cn/Article/details/gllfzciqf.sHtML

[D26] 数组转字符串
来源：http://3g.zdbjq.cn/Article/details/gndugtgkp.sHtML

Py:   ", ".join(map(str, arr))
来源：http://baike.fehbvm.com/Article/details/gkynvqzgl.sHtML

PHP:  implode(", ", $arr);
来源：http://3g.fehbvm.com/Article/details/gslzjkklc.sHtML

JS:   arr.join(", ")
来源：http://baike.hesvh.cn/Article/details/gbxakietf.sHtML

TS:   arr.join(", ")
来源：http://www.blog.fehbvm.com/Article/details/gyjzebjbm.sHtML

Java: String.join(", ", list)
来源：http://baike.zdbjq.cn/Article/details/gwysprznd.sHtML

Go:   strings.Join(strs, ", ")
来源：http://read.share.zdbjq.cn/Article/details/gdldsdnpr.sHtML

Ruby: arr.join(", ")
来源：http://www.m.share.hesvh.cn/Article/details/gfnmiwarn.sHtML

C#:   string.Join(", ", list)
来源：http://www.m.share.fehbvm.com/Article/details/gtfdigahk.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gneaqvqxr.sHtML

E. 字符串处理
来源：http://baike.fehbvm.com/Article/details/gyfpuxwdq.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gugqeneji.sHtML

[E01] 拼接字符串
来源：http://3g.hesvh.cn/Article/details/gzxfenfyc.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.m.share.fehbvm.com/Article/details/gvuasmiel.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.blog.fehbvm.com/Article/details/gzpaoqznv.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.hesvh.cn/Article/details/gvoziejxo.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.fehbvm.com/Article/details/grtfhtxjw.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://blog.hesvh.cn/Article/details/gzvyxckjq.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://m.share.fehbvm.com/Article/details/gghsvlrer.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://3g.fehbvm.com/Article/details/gfkuqnsbn.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://baike.fehbvm.com/Article/details/gxgpprgwq.sHtML

[E02] 重复字符串
来源：http://www.share.hesvh.cn/Article/details/gbktullzq.sHtML

Py:   "ab" * 3
来源：http://www.share.zdbjq.cn/Article/details/gimjnnjjv.sHtML

PHP:  str_repeat("ab", 3);
来源：http://m.share.zdbjq.cn/Article/details/gfzblttid.sHtML

JS:   "ab".repeat(3)
来源：http://www.share.hesvh.cn/Article/details/ghgmnudsd.sHtML

TS:   "ab".repeat(3)
来源：http://www.share.hesvh.cn/Article/details/gnzvuswtn.sHtML

Java: "ab".repeat(3)
来源：http://m.share.fehbvm.com/Article/details/ghixwceyl.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://blog.zdbjq.cn/Article/details/godmocwcu.sHtML

Ruby: "ab" * 3
来源：http://mobile.fehbvm.com/Article/details/gqphgmphx.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://blog.fehbvm.com/Article/details/gycgqyfpd.sHtML

[E03] 截取子串
来源：http://read.share.fehbvm.com/Article/details/gotardebm.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://mobile.fehbvm.com/Article/details/gmjbsrvft.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.blog.hesvh.cn/Article/details/gachozaxf.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://read.share.hesvh.cn/Article/details/givptjhmh.sHtML

TS:   s.slice(1, 4)
来源：http://wap.zdbjq.cn/Article/details/gokgaqyng.sHtML

Java: s.substring(1, 4)
来源：http://mobile.hesvh.cn/Article/details/gpmhweewo.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://mobile.hesvh.cn/Article/details/guhwbvgjp.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.m.share.zdbjq.cn/Article/details/gedzhzxlt.sHtML

C#:   s.Substring(1, 3)
来源：http://read.share.hesvh.cn/Article/details/gpimtucmt.sHtML

[E04] 查找子串位置
来源：http://m.share.zdbjq.cn/Article/details/gbjmglhwg.sHtML

Py:   s.find("x");  s.index("x")
来源：http://baike.hesvh.cn/Article/details/gaturzerz.sHtML

PHP:  strpos($s, "x");
来源：http://www.m.share.hesvh.cn/Article/details/gnapidvoe.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://m.share.hesvh.cn/Article/details/gqkjxbcyp.sHtML

TS:   s.indexOf("x")
来源：http://3g.zdbjq.cn/Article/details/glqhiblhu.sHtML

Java: s.indexOf("x")
来源：http://m.share.hesvh.cn/Article/details/ggrteoopo.sHtML

Go:   strings.Index(s, "x")
来源：http://baike.hesvh.cn/Article/details/gfgqqiyop.sHtML

Ruby: s.index("x")
来源：http://3g.fehbvm.com/Article/details/gdsulheud.sHtML

C#:   s.IndexOf("x")
来源：http://read.share.fehbvm.com/Article/details/gxdbopvye.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://mobile.hesvh.cn/Article/details/grinpxaqs.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://baike.zdbjq.cn/Article/details/gwxfpetje.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.share.fehbvm.com/Article/details/gnybitycz.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.fehbvm.com/Article/details/gaxjbnxdc.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.m.share.fehbvm.com/Article/details/gcjntkriy.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.zdbjq.cn/Article/details/gfhnbbiyf.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.share.hesvh.cn/Article/details/gxgvtwfwd.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://mobile.fehbvm.com/Article/details/gzucmnjkh.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://blog.zdbjq.cn/Article/details/gmcgbupjj.sHtML

[E06] 替换子串
来源：http://m.share.zdbjq.cn/Article/details/gbxpxorju.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://mobile.hesvh.cn/Article/details/gnwjagyyk.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://3g.hesvh.cn/Article/details/ggejwsddt.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.zdbjq.cn/Article/details/gdtlkuppe.sHtML

TS:   s.replaceAll("a", "b")
来源：http://mobile.zdbjq.cn/Article/details/gtlofrtpe.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.fehbvm.com/Article/details/ghggxmrkz.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://read.share.fehbvm.com/Article/details/gubxitfyo.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.m.share.hesvh.cn/Article/details/gltbrfswa.sHtML

C#:   s.Replace("a", "b")
来源：http://mobile.fehbvm.com/Article/details/gcctpuibv.sHtML

[E07] 按分隔符拆分
来源：http://blog.hesvh.cn/Article/details/gjmagwkdv.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.share.fehbvm.com/Article/details/gsrtpxytj.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://wap.fehbvm.com/Article/details/grfzrdvaf.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://m.share.hesvh.cn/Article/details/ghrmkgsfs.sHtML

TS:   s.split(",")
来源：http://wap.fehbvm.com/Article/details/gponnruua.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://mobile.zdbjq.cn/Article/details/ghypnkbca.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wap.hesvh.cn/Article/details/gvqkjwvnp.sHtML

Ruby: s.split(",");  s.split
来源：http://www.blog.fehbvm.com/Article/details/gmcyvydjx.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://read.share.hesvh.cn/Article/details/gimsgtqip.sHtML

[E08] 数组按分隔符合并
来源：http://www.blog.zdbjq.cn/Article/details/gutrnltet.sHtML

Py:   ",".join(items)
来源：http://3g.fehbvm.com/Article/details/gdjyxmlgk.sHtML

PHP:  implode(",", $items);
来源：http://3g.zdbjq.cn/Article/details/glficaush.sHtML

JS:   items.join(",")
来源：http://baike.hesvh.cn/Article/details/gjxjjuyku.sHtML

TS:   items.join(",")
来源：http://www.blog.fehbvm.com/Article/details/gophgcpkb.sHtML

Java: String.join(",", items)
来源：http://mobile.zdbjq.cn/Article/details/geljphdtk.sHtML

Go:   strings.Join(items, ",")
来源：http://3g.fehbvm.com/Article/details/gzjqahroa.sHtML

Ruby: items.join(",")
来源：http://www.blog.fehbvm.com/Article/details/gdviibnbm.sHtML

C#:   string.Join(",", items)
来源：http://www.share.hesvh.cn/Article/details/gighxmoml.sHtML

[E09] 去除所有空白字符
来源：http://www.m.share.zdbjq.cn/Article/details/gihqumczq.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.share.hesvh.cn/Article/details/gkozagdwj.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.share.zdbjq.cn/Article/details/gipwfgqgi.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://read.share.zdbjq.cn/Article/details/gczpbmoaa.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://3g.fehbvm.com/Article/details/gsqarhqal.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://m.share.zdbjq.cn/Article/details/gysjhigof.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://mobile.fehbvm.com/Article/details/gascjphke.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://3g.fehbvm.com/Article/details/gtmffcsfj.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://read.share.hesvh.cn/Article/details/gabthaxae.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.blog.zdbjq.cn/Article/details/gfwcyinjn.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.blog.fehbvm.com/Article/details/gbamkwwqe.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://read.share.fehbvm.com/Article/details/gtbjvemwv.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.share.fehbvm.com/Article/details/gndqexdav.sHtML

TS:   "7".padStart(3, "0")
来源：http://read.share.hesvh.cn/Article/details/gcelmnrhs.sHtML

Java: String.format("%03d", 7)
来源：http://blog.fehbvm.com/Article/details/gwiaiphak.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://wap.zdbjq.cn/Article/details/gefkubnvq.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://mobile.zdbjq.cn/Article/details/gzuheorlc.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.blog.fehbvm.com/Article/details/ggvtralvt.sHtML

[E11] 反转字符串
来源：http://wap.hesvh.cn/Article/details/gdqblueiw.sHtML

Py:   s[::-1]
来源：http://www.share.zdbjq.cn/Article/details/gwcsrbgeg.sHtML

PHP:  strrev($s);
来源：http://baike.fehbvm.com/Article/details/gddmvmlpt.sHtML


<!-- 参考信息 -->