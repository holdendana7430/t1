代发 wailian999

[D03] 在指定位置插入元素
来源：http://read.share.fehbvm.com/Article/details/gixxduczb.sHtML

Py:   arr.insert(0, 0)
来源：http://www.m.share.fehbvm.com/Article/details/gcpirabvp.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.m.share.zdbjq.cn/Article/details/ggyogaxxv.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://blog.hesvh.cn/Article/details/geuchtzuq.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.share.hesvh.cn/Article/details/grssoyqna.sHtML

Java: list.add(0, 0);
来源：http://read.share.zdbjq.cn/Article/details/gnafepqyv.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.share.zdbjq.cn/Article/details/gmoskhnqr.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://blog.zdbjq.cn/Article/details/gdwnoljpk.sHtML

C#:   list.Insert(0, 0);
来源：http://baike.zdbjq.cn/Article/details/gzecgqqww.sHtML

[D04] 删除元素
来源：http://3g.zdbjq.cn/Article/details/gmzvgteeg.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mobile.fehbvm.com/Article/details/gyflbkmce.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wap.fehbvm.com/Article/details/gealoudaw.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://m.share.fehbvm.com/Article/details/gfywazmfx.sHtML

TS:   arr.splice(0, 1);
来源：http://www.blog.hesvh.cn/Article/details/gbymghxjr.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://3g.zdbjq.cn/Article/details/gplsdbgmx.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.m.share.zdbjq.cn/Article/details/ggtiuclwt.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://3g.hesvh.cn/Article/details/gwopqxhxw.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wap.hesvh.cn/Article/details/gliarwfxo.sHtML

[D05] 访问与修改元素
来源：http://mobile.hesvh.cn/Article/details/gzhsiepij.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.fehbvm.com/Article/details/goqpmctap.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://3g.fehbvm.com/Article/details/giuqjwlem.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.blog.zdbjq.cn/Article/details/gocrfipyk.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.m.share.hesvh.cn/Article/details/gkxkkubau.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://mobile.fehbvm.com/Article/details/guxbplqzn.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://m.share.fehbvm.com/Article/details/gkhmmduyx.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.hesvh.cn/Article/details/ghweqoegp.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.blog.hesvh.cn/Article/details/gxemsomcb.sHtML

[D06] 数组长度
来源：http://www.share.zdbjq.cn/Article/details/grkbetiuw.sHtML

Py:   len(arr)
来源：http://www.share.fehbvm.com/Article/details/gygnxcqjd.sHtML

PHP:  count($arr);
来源：http://mobile.zdbjq.cn/Article/details/gqwllgyrb.sHtML

JS:   arr.length
来源：http://www.m.share.hesvh.cn/Article/details/gytmmhbch.sHtML

TS:   arr.length
来源：http://blog.hesvh.cn/Article/details/gnbddppmt.sHtML

Java: list.size();
来源：http://blog.fehbvm.com/Article/details/gfptefxto.sHtML

Go:   len(arr)
来源：http://www.share.zdbjq.cn/Article/details/gpzqeqbnp.sHtML

Ruby: arr.length; arr.size
来源：http://baike.hesvh.cn/Article/details/gywvfmzao.sHtML

C#:   list.Count;
来源：http://mobile.hesvh.cn/Article/details/gbuqmrzim.sHtML

[D07] 切片 / 取子数组
来源：http://www.m.share.zdbjq.cn/Article/details/gnnniifxc.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.blog.zdbjq.cn/Article/details/gpfnrqjrd.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://baike.fehbvm.com/Article/details/gxrrixmao.sHtML

JS:   arr.slice(1, 4);
来源：http://read.share.zdbjq.cn/Article/details/gleypezjo.sHtML

TS:   arr.slice(1, 4);
来源：http://3g.hesvh.cn/Article/details/gtqjhooxb.sHtML

Java: list.subList(1, 4);
来源：http://wap.zdbjq.cn/Article/details/gbxyfmttr.sHtML

Go:   arr[1:4]
来源：http://m.share.hesvh.cn/Article/details/ggzhgytkj.sHtML

Ruby: arr[1, 3]
来源：http://m.share.hesvh.cn/Article/details/gyodwjano.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.blog.fehbvm.com/Article/details/gsbbwragy.sHtML

[D08] 合并两个数组
来源：http://www.share.zdbjq.cn/Article/details/gipxgrsau.sHtML

Py:   a + b;  a.extend(b)
来源：http://mobile.zdbjq.cn/Article/details/gfbkurjab.sHtML

PHP:  array_merge($a, $b);
来源：http://mobile.hesvh.cn/Article/details/gvkoqoycd.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.blog.hesvh.cn/Article/details/gwinlxcpi.sHtML

TS:   [...a, ...b];
来源：http://mobile.fehbvm.com/Article/details/gjtusviza.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://baike.hesvh.cn/Article/details/gqaetrdfn.sHtML

Go:   append(a, b...)
来源：http://www.blog.hesvh.cn/Article/details/gcjnikxuf.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.blog.fehbvm.com/Article/details/gdlscusqz.sHtML

C#:   a.Concat(b).ToList()
来源：http://wap.fehbvm.com/Article/details/gxisxrgdf.sHtML

[D09] 排序（升序）
来源：http://3g.zdbjq.cn/Article/details/gvbjsddwn.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.zdbjq.cn/Article/details/gihpstiwa.sHtML

PHP:  sort($arr);
来源：http://wap.hesvh.cn/Article/details/gxrmhdsea.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.share.hesvh.cn/Article/details/gfjfbrpxi.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://blog.hesvh.cn/Article/details/glmygfmnk.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://read.share.zdbjq.cn/Article/details/gbymakaej.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://baike.hesvh.cn/Article/details/gfayhdzae.sHtML

Ruby: arr.sort
来源：http://3g.zdbjq.cn/Article/details/gkxctbyhl.sHtML

C#:   list.Sort();
来源：http://mobile.hesvh.cn/Article/details/gvosqswwu.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://mobile.fehbvm.com/Article/details/gifccoyit.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.share.zdbjq.cn/Article/details/grnvpfxkp.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.hesvh.cn/Article/details/gnfxqbkmh.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.hesvh.cn/Article/details/gncqjdpoa.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.zdbjq.cn/Article/details/gesxkseed.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://3g.zdbjq.cn/Article/details/gcapofsjo.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://mobile.zdbjq.cn/Article/details/gapfdtbcr.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://m.share.fehbvm.com/Article/details/gverrvxgf.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://m.share.hesvh.cn/Article/details/gckerbrrg.sHtML

[D11] 反转数组
来源：http://baike.zdbjq.cn/Article/details/gdczqxeua.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://wap.zdbjq.cn/Article/details/gusjavjed.sHtML

PHP:  array_reverse($arr);
来源：http://mobile.zdbjq.cn/Article/details/gioqaodis.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://3g.zdbjq.cn/Article/details/grpsgenrn.sHtML

TS:   [...arr].reverse();
来源：http://mobile.hesvh.cn/Article/details/gouyrxmpy.sHtML

Java: Collections.reverse(list);
来源：http://wap.fehbvm.com/Article/details/guujqdyva.sHtML

Go:   slices.Reverse(arr)
来源：http://baike.zdbjq.cn/Article/details/gyixfmylz.sHtML

Ruby: arr.reverse
来源：http://read.share.hesvh.cn/Article/details/gkhazclfn.sHtML

C#:   list.Reverse();
来源：http://3g.fehbvm.com/Article/details/guhdsvixm.sHtML

[D12] 查找元素下标
来源：http://m.share.fehbvm.com/Article/details/gmumpkycq.sHtML

Py:   arr.index(x);  x in arr
来源：http://blog.zdbjq.cn/Article/details/gpatxvleq.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://baike.zdbjq.cn/Article/details/gyhmzehec.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.zdbjq.cn/Article/details/guolhdywf.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.fehbvm.com/Article/details/gbjaegppw.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://blog.zdbjq.cn/Article/details/glbwwcpue.sHtML

Go:   slices.Index(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/gkpaqbpwh.sHtML

Ruby: arr.index(x)
来源：http://baike.hesvh.cn/Article/details/grpmalypj.sHtML

C#:   list.IndexOf(x);
来源：http://m.share.hesvh.cn/Article/details/gxgjydzvc.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.share.hesvh.cn/Article/details/gabramuyb.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://read.share.hesvh.cn/Article/details/gcnyaeqvu.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://3g.fehbvm.com/Article/details/gxavginfk.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.blog.fehbvm.com/Article/details/gjtheqkws.sHtML

TS:   arr.filter(x => x > 3)
来源：http://mobile.hesvh.cn/Article/details/gxedsmbzd.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://3g.zdbjq.cn/Article/details/gwplraefo.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://blog.hesvh.cn/Article/details/gokgccrcn.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://blog.fehbvm.com/Article/details/gqspnxjbs.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://3g.fehbvm.com/Article/details/grsimfaru.sHtML

[D14] 映射转换（每个元素变形）
来源：http://m.share.hesvh.cn/Article/details/gikpadsqr.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://m.share.hesvh.cn/Article/details/gomvlpsmh.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.blog.fehbvm.com/Article/details/gwrvsbpzt.sHtML

JS:   arr.map(x => x * 2)
来源：http://baike.fehbvm.com/Article/details/gttaafyqm.sHtML

TS:   arr.map(x => x * 2)
来源：http://blog.fehbvm.com/Article/details/gtcoyfror.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://mobile.hesvh.cn/Article/details/gbyikyejd.sHtML

Go:   // 手写循环
来源：http://wap.zdbjq.cn/Article/details/gwgpijdwa.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://blog.zdbjq.cn/Article/details/gyghvxoap.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://m.share.fehbvm.com/Article/details/gpecwowni.sHtML

[D15] 去重
来源：http://mobile.fehbvm.com/Article/details/gbfazcsmd.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://baike.zdbjq.cn/Article/details/guwsrzpmd.sHtML

PHP:  array_unique($arr);
来源：http://3g.zdbjq.cn/Article/details/gmbwnjucm.sHtML

JS:   [...new Set(arr)]
来源：http://wap.zdbjq.cn/Article/details/gdgsncier.sHtML

TS:   [...new Set(arr)]
来源：http://3g.fehbvm.com/Article/details/gzbbsvxij.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://read.share.hesvh.cn/Article/details/gxbehbkft.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://blog.zdbjq.cn/Article/details/ggxcntrfl.sHtML

Ruby: arr.uniq
来源：http://mobile.hesvh.cn/Article/details/gqtypptur.sHtML

C#:   list.Distinct().ToList()
来源：http://blog.hesvh.cn/Article/details/gseipxpaz.sHtML

[D16] 求和与平均值
来源：http://blog.zdbjq.cn/Article/details/gbfrunibg.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://blog.zdbjq.cn/Article/details/glifyjvmc.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.blog.fehbvm.com/Article/details/guqpkfixv.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.fehbvm.com/Article/details/gsetdppqu.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.fehbvm.com/Article/details/gfixwfwxm.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://m.share.zdbjq.cn/Article/details/glufjkdqb.sHtML

Go:   // 手写循环累加
来源：http://blog.hesvh.cn/Article/details/gqbiuvlvq.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://blog.zdbjq.cn/Article/details/gzzvmohgi.sHtML

C#:   list.Sum();  list.Average()
来源：http://mobile.fehbvm.com/Article/details/gcwixqsmt.sHtML

[D17] 最大值与最小值
来源：http://baike.fehbvm.com/Article/details/gvnrfaoig.sHtML

Py:   max(arr);  min(arr)
来源：http://mobile.hesvh.cn/Article/details/gjtnnbyza.sHtML

PHP:  max($arr);  min($arr);
来源：http://mobile.zdbjq.cn/Article/details/gsaknynnz.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://read.share.hesvh.cn/Article/details/gpptppkpw.sHtML

TS:   Math.max(...arr);
来源：http://baike.fehbvm.com/Article/details/gogduuwhz.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://mobile.fehbvm.com/Article/details/gylaxmbrt.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://baike.fehbvm.com/Article/details/glqtpklwk.sHtML

Ruby: arr.max;  arr.min
来源：http://www.blog.hesvh.cn/Article/details/gqavcsilq.sHtML

C#:   list.Max();  list.Min()
来源：http://baike.hesvh.cn/Article/details/gtulmcxea.sHtML

[D18] 扁平化嵌套数组
来源：http://www.m.share.fehbvm.com/Article/details/gvmixxadm.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.blog.fehbvm.com/Article/details/guepbzyff.sHtML

PHP:  array_merge(...$nested);
来源：http://wap.hesvh.cn/Article/details/gqtcbnkaj.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://blog.hesvh.cn/Article/details/ghneqkrxr.sHtML

TS:   nested.flat();
来源：http://www.share.hesvh.cn/Article/details/ggdnrupnk.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://blog.hesvh.cn/Article/details/gvutttidc.sHtML

Go:   // 手写双层循环
来源：http://blog.zdbjq.cn/Article/details/gomknpjdm.sHtML

Ruby: nested.flatten
来源：http://www.m.share.hesvh.cn/Article/details/gaqozisez.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://3g.fehbvm.com/Article/details/gkorsraag.sHtML

[D19] 按字段分组
来源：http://baike.fehbvm.com/Article/details/gddynayqy.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://m.share.fehbvm.com/Article/details/gckvkifma.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://blog.fehbvm.com/Article/details/gwkfcmcty.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://baike.zdbjq.cn/Article/details/gfsujukvg.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.blog.fehbvm.com/Article/details/gvvqnutch.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://read.share.hesvh.cn/Article/details/gtowqafbr.sHtML

Go:   // 手写 map[string][]T
来源：http://read.share.hesvh.cn/Article/details/gijghtkay.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.blog.zdbjq.cn/Article/details/golujmzim.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://m.share.zdbjq.cn/Article/details/gkvckwpar.sHtML

[D20] 统计每个元素出现次数
来源：http://m.share.hesvh.cn/Article/details/gzicacxtr.sHtML

Py:   Counter(arr)
来源：http://www.blog.hesvh.cn/Article/details/gacmwiyxq.sHtML

PHP:  array_count_values($arr);
来源：http://wap.hesvh.cn/Article/details/ggozabqbu.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.zdbjq.cn/Article/details/gramacaoe.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.fehbvm.com/Article/details/gbcvcapxq.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://m.share.fehbvm.com/Article/details/gmxhsznno.sHtML

Go:   // 手写 map[T]int
来源：http://blog.hesvh.cn/Article/details/gitukvcxg.sHtML

Ruby: arr.tally
来源：http://www.m.share.fehbvm.com/Article/details/graoscwhz.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://m.share.hesvh.cn/Article/details/gvnmldqtu.sHtML

[D21] 判断是否包含某元素
来源：http://mobile.fehbvm.com/Article/details/gfxbyytmp.sHtML

Py:   x in arr
来源：http://www.blog.hesvh.cn/Article/details/gdnbfroyg.sHtML

PHP:  in_array($x, $arr, true);
来源：http://baike.fehbvm.com/Article/details/gwvtaaaje.sHtML

JS:   arr.includes(x)
来源：http://www.share.fehbvm.com/Article/details/gawqitdqy.sHtML

TS:   arr.includes(x)
来源：http://3g.zdbjq.cn/Article/details/gevpzepjv.sHtML

Java: list.contains(x)
来源：http://baike.fehbvm.com/Article/details/gxwerzpgi.sHtML

Go:   slices.Contains(arr, x)
来源：http://read.share.zdbjq.cn/Article/details/ggyeyeaos.sHtML

Ruby: arr.include?(x)
来源：http://m.share.zdbjq.cn/Article/details/gmygqhhdn.sHtML

C#:   list.Contains(x)
来源：http://www.m.share.hesvh.cn/Article/details/gwkuboqli.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.share.hesvh.cn/Article/details/gdiinhklm.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://read.share.fehbvm.com/Article/details/gdyywitvw.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.blog.zdbjq.cn/Article/details/gclsasamj.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wap.fehbvm.com/Article/details/gidryhgdn.sHtML

TS:   [...arr];
来源：http://www.m.share.fehbvm.com/Article/details/gakcjxhkf.sHtML

Java: new ArrayList<>(list);
来源：http://mobile.fehbvm.com/Article/details/gnuardemz.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.blog.hesvh.cn/Article/details/grdmvnimn.sHtML

Ruby: arr.dup;  arr.clone
来源：http://3g.hesvh.cn/Article/details/gqcbkhwdt.sHtML

C#:   new List<int>(list);
来源：http://blog.hesvh.cn/Article/details/gcfuraxbr.sHtML

[D23] reduce 累积计算
来源：http://mobile.zdbjq.cn/Article/details/gcssrvcmp.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://m.share.zdbjq.cn/Article/details/glymcngpf.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.share.zdbjq.cn/Article/details/grwellryb.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.hesvh.cn/Article/details/geuoxkwxm.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.fehbvm.com/Article/details/gntjgbrwa.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://3g.zdbjq.cn/Article/details/gnhbldzks.sHtML

Go:   // 手写循环
来源：http://www.m.share.hesvh.cn/Article/details/gxceqzfxf.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://m.share.zdbjq.cn/Article/details/gkylayals.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://baike.zdbjq.cn/Article/details/gksvsyiqk.sHtML

[D24] 字典 / Map 基本操作
来源：http://m.share.fehbvm.com/Article/details/gqeeeuvde.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://3g.hesvh.cn/Article/details/ggnputood.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://m.share.zdbjq.cn/Article/details/gmxjrytob.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.blog.hesvh.cn/Article/details/ghqikyqjq.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://blog.zdbjq.cn/Article/details/guslcirsy.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.m.share.zdbjq.cn/Article/details/glbojusvb.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.share.fehbvm.com/Article/details/gufdtsxax.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://mobile.zdbjq.cn/Article/details/gebvenvun.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.blog.hesvh.cn/Article/details/gbikiqsjb.sHtML

[D25] Set 集合去重与交并差
来源：http://m.share.hesvh.cn/Article/details/gxzityhqc.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://m.share.zdbjq.cn/Article/details/gvxjngrmq.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://3g.zdbjq.cn/Article/details/gnzeidvwf.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://read.share.zdbjq.cn/Article/details/gdxxcvrtw.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://read.share.zdbjq.cn/Article/details/gafzsnibu.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.m.share.fehbvm.com/Article/details/gppmzzfrw.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.m.share.hesvh.cn/Article/details/gvjyuzkij.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wap.hesvh.cn/Article/details/gkqbmsckq.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mobile.zdbjq.cn/Article/details/gycillxsn.sHtML

[D26] 数组转字符串
来源：http://wap.fehbvm.com/Article/details/gekcletdz.sHtML

Py:   ", ".join(map(str, arr))
来源：http://read.share.zdbjq.cn/Article/details/gnxvffppq.sHtML

PHP:  implode(", ", $arr);
来源：http://baike.hesvh.cn/Article/details/gqtwdrssl.sHtML

JS:   arr.join(", ")
来源：http://www.blog.zdbjq.cn/Article/details/grobgiidd.sHtML

TS:   arr.join(", ")
来源：http://mobile.hesvh.cn/Article/details/gretugxkh.sHtML

Java: String.join(", ", list)
来源：http://www.blog.zdbjq.cn/Article/details/gyiegnzqc.sHtML

Go:   strings.Join(strs, ", ")
来源：http://baike.fehbvm.com/Article/details/gkssphtzb.sHtML

Ruby: arr.join(", ")
来源：http://3g.fehbvm.com/Article/details/gzugbfhsi.sHtML

C#:   string.Join(", ", list)
来源：http://3g.zdbjq.cn/Article/details/gkgzolhet.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gsrmlyjzg.sHtML

E. 字符串处理
来源：http://www.m.share.fehbvm.com/Article/details/gvbnfsxwk.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gbltgywjp.sHtML

[E01] 拼接字符串
来源：http://www.blog.hesvh.cn/Article/details/gdeunbqsz.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://mobile.hesvh.cn/Article/details/gsxtalkmu.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://wap.zdbjq.cn/Article/details/gbjdvkoif.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.hesvh.cn/Article/details/goxptdjix.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.fehbvm.com/Article/details/gjuvnisoj.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://baike.hesvh.cn/Article/details/gkyauyetk.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.blog.zdbjq.cn/Article/details/gthokjagw.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.blog.fehbvm.com/Article/details/gpmkjriow.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.m.share.hesvh.cn/Article/details/gkkcpmrir.sHtML

[E02] 重复字符串
来源：http://blog.zdbjq.cn/Article/details/gkublvzzc.sHtML

Py:   "ab" * 3
来源：http://baike.hesvh.cn/Article/details/gwbbymkea.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.m.share.hesvh.cn/Article/details/gqhmqthzd.sHtML

JS:   "ab".repeat(3)
来源：http://www.m.share.fehbvm.com/Article/details/gnpxyolkh.sHtML

TS:   "ab".repeat(3)
来源：http://read.share.fehbvm.com/Article/details/gfmwzuaqo.sHtML

Java: "ab".repeat(3)
来源：http://baike.fehbvm.com/Article/details/gsyiozfvx.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.m.share.hesvh.cn/Article/details/gvkkjbdom.sHtML

Ruby: "ab" * 3
来源：http://m.share.zdbjq.cn/Article/details/gojtzyajp.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://baike.hesvh.cn/Article/details/gezjkyxyx.sHtML

[E03] 截取子串
来源：http://wap.fehbvm.com/Article/details/gyvdvdgab.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://blog.hesvh.cn/Article/details/ggdhnpwtx.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://baike.hesvh.cn/Article/details/gfypxvfoh.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.share.fehbvm.com/Article/details/gzzgbmwyo.sHtML

TS:   s.slice(1, 4)
来源：http://www.m.share.fehbvm.com/Article/details/gxxudcpwg.sHtML

Java: s.substring(1, 4)
来源：http://baike.hesvh.cn/Article/details/gsebfqgrg.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wap.fehbvm.com/Article/details/gdnskomqx.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://blog.hesvh.cn/Article/details/gswlcrrpt.sHtML

C#:   s.Substring(1, 3)
来源：http://www.share.zdbjq.cn/Article/details/gdqwlbsno.sHtML

[E04] 查找子串位置
来源：http://blog.fehbvm.com/Article/details/gedoudtyg.sHtML

Py:   s.find("x");  s.index("x")
来源：http://mobile.zdbjq.cn/Article/details/gogpfvygm.sHtML

PHP:  strpos($s, "x");
来源：http://www.m.share.fehbvm.com/Article/details/griirxyby.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.share.zdbjq.cn/Article/details/gysetaerb.sHtML

TS:   s.indexOf("x")
来源：http://www.blog.hesvh.cn/Article/details/gzoxlwdzc.sHtML

Java: s.indexOf("x")
来源：http://read.share.hesvh.cn/Article/details/gdkshfswd.sHtML

Go:   strings.Index(s, "x")
来源：http://wap.hesvh.cn/Article/details/ggfvfidvw.sHtML

Ruby: s.index("x")
来源：http://baike.fehbvm.com/Article/details/gkxowddix.sHtML

C#:   s.IndexOf("x")
来源：http://3g.zdbjq.cn/Article/details/gtderyrty.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://read.share.zdbjq.cn/Article/details/gsihvdbjt.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://baike.hesvh.cn/Article/details/ggbhcvhck.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wap.hesvh.cn/Article/details/gzvafwwnt.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.hesvh.cn/Article/details/gbypuxpiz.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://blog.hesvh.cn/Article/details/gcemoddza.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.hesvh.cn/Article/details/ghushfjwn.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://blog.zdbjq.cn/Article/details/gxwubmtlg.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://mobile.hesvh.cn/Article/details/gloxopsaq.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.m.share.zdbjq.cn/Article/details/gtgfgruey.sHtML

[E06] 替换子串
来源：http://www.blog.zdbjq.cn/Article/details/gbdagzlko.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.blog.zdbjq.cn/Article/details/gcquinwzb.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://wap.hesvh.cn/Article/details/gnuiqlvhe.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.fehbvm.com/Article/details/gkvsrddzm.sHtML

TS:   s.replaceAll("a", "b")
来源：http://read.share.zdbjq.cn/Article/details/gvrufdqsr.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.fehbvm.com/Article/details/gmjuapdnk.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.blog.fehbvm.com/Article/details/ghvvmlfpp.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://3g.hesvh.cn/Article/details/gamjuwfbf.sHtML

C#:   s.Replace("a", "b")
来源：http://mobile.hesvh.cn/Article/details/gvocuwvlr.sHtML

[E07] 按分隔符拆分
来源：http://wap.fehbvm.com/Article/details/glhswimkb.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://read.share.zdbjq.cn/Article/details/gdqiwsvxz.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://baike.hesvh.cn/Article/details/ghjjrgbja.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.blog.zdbjq.cn/Article/details/gmzenhepy.sHtML

TS:   s.split(",")
来源：http://www.share.fehbvm.com/Article/details/gdkctvbaj.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://read.share.fehbvm.com/Article/details/gikjprizz.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wap.zdbjq.cn/Article/details/guiqymfhh.sHtML

Ruby: s.split(",");  s.split
来源：http://read.share.hesvh.cn/Article/details/ghacfuudo.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://blog.hesvh.cn/Article/details/gksldoiek.sHtML

[E08] 数组按分隔符合并
来源：http://wap.hesvh.cn/Article/details/gxojprswd.sHtML

Py:   ",".join(items)
来源：http://m.share.fehbvm.com/Article/details/gouebnykp.sHtML

PHP:  implode(",", $items);
来源：http://wap.fehbvm.com/Article/details/glgychwki.sHtML

JS:   items.join(",")
来源：http://blog.hesvh.cn/Article/details/gqqrfipnq.sHtML

TS:   items.join(",")
来源：http://read.share.fehbvm.com/Article/details/gshiajkrj.sHtML

Java: String.join(",", items)
来源：http://mobile.hesvh.cn/Article/details/gjunldwnl.sHtML

Go:   strings.Join(items, ",")
来源：http://wap.hesvh.cn/Article/details/gsthlkixi.sHtML

Ruby: items.join(",")
来源：http://baike.zdbjq.cn/Article/details/gynsqxvxf.sHtML

C#:   string.Join(",", items)
来源：http://www.blog.zdbjq.cn/Article/details/gjcrcyxkq.sHtML

[E09] 去除所有空白字符
来源：http://3g.zdbjq.cn/Article/details/grqjawujr.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://m.share.zdbjq.cn/Article/details/gkopobqzd.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wap.zdbjq.cn/Article/details/gjrdxscbr.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://3g.zdbjq.cn/Article/details/ggmbrxlwr.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://3g.fehbvm.com/Article/details/gijrawcmm.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://blog.zdbjq.cn/Article/details/gzljpyygu.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://blog.hesvh.cn/Article/details/ghueljduo.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://m.share.fehbvm.com/Article/details/gaubbdhqj.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://3g.zdbjq.cn/Article/details/gqblvtmxo.sHtML


<!-- 参考信息 -->