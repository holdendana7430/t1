代发 wailian999

Py:   len(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gylkouqfp.sHtML

PHP:  count($arr);
来源：http://blog.zdbjq.cn/Article/details/gophyzqiy.sHtML

JS:   arr.length
来源：http://baike.hesvh.cn/Article/details/gioolpwma.sHtML

TS:   arr.length
来源：http://3g.hesvh.cn/Article/details/gmcdryvxq.sHtML

Java: list.size();
来源：http://www.m.share.fehbvm.com/Article/details/ghtjfrxpy.sHtML

Go:   len(arr)
来源：http://read.share.zdbjq.cn/Article/details/ghzekebwn.sHtML

Ruby: arr.length; arr.size
来源：http://baike.zdbjq.cn/Article/details/gefjhlxpg.sHtML

C#:   list.Count;
来源：http://blog.zdbjq.cn/Article/details/gxgvwcfns.sHtML

[D07] 切片 / 取子数组
来源：http://wap.fehbvm.com/Article/details/gtfjuvhbz.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://m.share.fehbvm.com/Article/details/gqtqliewi.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://wap.fehbvm.com/Article/details/gsqkeofce.sHtML

JS:   arr.slice(1, 4);
来源：http://m.share.hesvh.cn/Article/details/goonakaqt.sHtML

TS:   arr.slice(1, 4);
来源：http://read.share.zdbjq.cn/Article/details/gcbtvdcln.sHtML

Java: list.subList(1, 4);
来源：http://www.share.fehbvm.com/Article/details/gfzmzisbx.sHtML

Go:   arr[1:4]
来源：http://www.blog.zdbjq.cn/Article/details/gssojrwbo.sHtML

Ruby: arr[1, 3]
来源：http://www.blog.fehbvm.com/Article/details/gtyltieer.sHtML

C#:   list.GetRange(1, 3);
来源：http://mobile.zdbjq.cn/Article/details/gnaxxuove.sHtML

[D08] 合并两个数组
来源：http://www.m.share.zdbjq.cn/Article/details/ghloulwub.sHtML

Py:   a + b;  a.extend(b)
来源：http://m.share.hesvh.cn/Article/details/gxwhjjyhe.sHtML

PHP:  array_merge($a, $b);
来源：http://baike.fehbvm.com/Article/details/gbncxiojd.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.share.hesvh.cn/Article/details/ghljjbigu.sHtML

TS:   [...a, ...b];
来源：http://www.m.share.hesvh.cn/Article/details/gqswfkarn.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://3g.hesvh.cn/Article/details/gexpjrabh.sHtML

Go:   append(a, b...)
来源：http://blog.zdbjq.cn/Article/details/giskfczah.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.m.share.zdbjq.cn/Article/details/gtddtodxi.sHtML

C#:   a.Concat(b).ToList()
来源：http://baike.fehbvm.com/Article/details/gpnytnwps.sHtML

[D09] 排序（升序）
来源：http://www.m.share.fehbvm.com/Article/details/gsxxzcses.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.zdbjq.cn/Article/details/gwmesbvvq.sHtML

PHP:  sort($arr);
来源：http://read.share.zdbjq.cn/Article/details/gxbxpizgd.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.m.share.hesvh.cn/Article/details/gopiozhlo.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.share.fehbvm.com/Article/details/gtlflqkub.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.m.share.zdbjq.cn/Article/details/gkswjoleq.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.blog.zdbjq.cn/Article/details/glivtbmsn.sHtML

Ruby: arr.sort
来源：http://www.share.hesvh.cn/Article/details/gntwwvahf.sHtML

C#:   list.Sort();
来源：http://blog.zdbjq.cn/Article/details/gietnagpm.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://blog.hesvh.cn/Article/details/gzsvrauye.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://baike.hesvh.cn/Article/details/gfucmmufu.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.hesvh.cn/Article/details/gmfyyxplx.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.fehbvm.com/Article/details/gvqputtpp.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.fehbvm.com/Article/details/gqihbjmwy.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://blog.zdbjq.cn/Article/details/gruzfzzri.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.blog.fehbvm.com/Article/details/gycfcvfbn.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://3g.hesvh.cn/Article/details/gbwuigahs.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://baike.fehbvm.com/Article/details/glgmitphw.sHtML

[D11] 反转数组
来源：http://baike.fehbvm.com/Article/details/gkpwidyyu.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://wap.hesvh.cn/Article/details/ggokhbkuv.sHtML

PHP:  array_reverse($arr);
来源：http://baike.zdbjq.cn/Article/details/gkhvdxplc.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.blog.hesvh.cn/Article/details/gtvtsfxkb.sHtML

TS:   [...arr].reverse();
来源：http://baike.zdbjq.cn/Article/details/gnemvxsfe.sHtML

Java: Collections.reverse(list);
来源：http://baike.hesvh.cn/Article/details/gprimuori.sHtML

Go:   slices.Reverse(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gmbawmfaq.sHtML

Ruby: arr.reverse
来源：http://read.share.fehbvm.com/Article/details/gdphubdeh.sHtML

C#:   list.Reverse();
来源：http://blog.fehbvm.com/Article/details/gdokwpkyx.sHtML

[D12] 查找元素下标
来源：http://3g.hesvh.cn/Article/details/gbqziudar.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.m.share.zdbjq.cn/Article/details/gxqlqpnrx.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://m.share.zdbjq.cn/Article/details/gkhlzsxgr.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.zdbjq.cn/Article/details/gsdzkakaz.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.zdbjq.cn/Article/details/gfeiqxktz.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://blog.zdbjq.cn/Article/details/ghvcraidf.sHtML

Go:   slices.Index(arr, x)
来源：http://www.blog.fehbvm.com/Article/details/gbhpccqza.sHtML

Ruby: arr.index(x)
来源：http://3g.hesvh.cn/Article/details/groafmhaa.sHtML

C#:   list.IndexOf(x);
来源：http://baike.zdbjq.cn/Article/details/gcfqutier.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.m.share.fehbvm.com/Article/details/gbabawjvp.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://baike.fehbvm.com/Article/details/glnxbzfys.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://read.share.hesvh.cn/Article/details/geohddyil.sHtML

JS:   arr.filter(x => x > 3)
来源：http://m.share.zdbjq.cn/Article/details/gogzunwgi.sHtML

TS:   arr.filter(x => x > 3)
来源：http://blog.hesvh.cn/Article/details/gbgpzanxc.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.m.share.fehbvm.com/Article/details/gntuckxcs.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://blog.hesvh.cn/Article/details/gtpbrpkek.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.blog.zdbjq.cn/Article/details/ggvbnciik.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://wap.fehbvm.com/Article/details/groymgnlv.sHtML

[D14] 映射转换（每个元素变形）
来源：http://mobile.fehbvm.com/Article/details/gmoaqplht.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://m.share.fehbvm.com/Article/details/grsqciisi.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.blog.hesvh.cn/Article/details/gygsjzytc.sHtML

JS:   arr.map(x => x * 2)
来源：http://m.share.fehbvm.com/Article/details/gwdkrvkui.sHtML

TS:   arr.map(x => x * 2)
来源：http://blog.hesvh.cn/Article/details/gmkwgernd.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.m.share.zdbjq.cn/Article/details/guhdmktad.sHtML

Go:   // 手写循环
来源：http://mobile.hesvh.cn/Article/details/gdsnpbtvp.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://read.share.fehbvm.com/Article/details/glkhwrnvl.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://blog.fehbvm.com/Article/details/genycegth.sHtML

[D15] 去重
来源：http://www.m.share.fehbvm.com/Article/details/gmldanrlj.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.m.share.fehbvm.com/Article/details/gzmxzecic.sHtML

PHP:  array_unique($arr);
来源：http://read.share.zdbjq.cn/Article/details/ghfwtcbuv.sHtML

JS:   [...new Set(arr)]
来源：http://blog.hesvh.cn/Article/details/gfkwyzvax.sHtML

TS:   [...new Set(arr)]
来源：http://www.share.zdbjq.cn/Article/details/gmaeiajxe.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://3g.zdbjq.cn/Article/details/gcftlymkn.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.blog.zdbjq.cn/Article/details/gcjdduwqf.sHtML

Ruby: arr.uniq
来源：http://www.blog.zdbjq.cn/Article/details/gjqcbefho.sHtML

C#:   list.Distinct().ToList()
来源：http://www.blog.hesvh.cn/Article/details/gygijoyfl.sHtML

[D16] 求和与平均值
来源：http://baike.zdbjq.cn/Article/details/gigupnpin.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://blog.zdbjq.cn/Article/details/glfcitxbd.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mobile.hesvh.cn/Article/details/gvghetdzq.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.hesvh.cn/Article/details/gawttzloa.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.fehbvm.com/Article/details/gqkdktsnu.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://read.share.fehbvm.com/Article/details/gjxswdvks.sHtML

Go:   // 手写循环累加
来源：http://3g.zdbjq.cn/Article/details/gqtpxpvrh.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://baike.fehbvm.com/Article/details/gydhyphyz.sHtML

C#:   list.Sum();  list.Average()
来源：http://m.share.zdbjq.cn/Article/details/gjoittttn.sHtML

[D17] 最大值与最小值
来源：http://www.m.share.fehbvm.com/Article/details/ghuymcvyw.sHtML

Py:   max(arr);  min(arr)
来源：http://www.blog.hesvh.cn/Article/details/gkqqvqkjf.sHtML

PHP:  max($arr);  min($arr);
来源：http://read.share.fehbvm.com/Article/details/gjaghcpqz.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wap.fehbvm.com/Article/details/gudhrbmak.sHtML

TS:   Math.max(...arr);
来源：http://3g.zdbjq.cn/Article/details/gxjterins.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://blog.zdbjq.cn/Article/details/grtakdvol.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://baike.hesvh.cn/Article/details/gqfvwhiry.sHtML

Ruby: arr.max;  arr.min
来源：http://read.share.fehbvm.com/Article/details/gsuwznnqt.sHtML

C#:   list.Max();  list.Min()
来源：http://m.share.fehbvm.com/Article/details/gcbwaexhf.sHtML

[D18] 扁平化嵌套数组
来源：http://www.m.share.hesvh.cn/Article/details/gpodyurdn.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.m.share.fehbvm.com/Article/details/gzvaliufw.sHtML

PHP:  array_merge(...$nested);
来源：http://3g.fehbvm.com/Article/details/gkywppsew.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mobile.hesvh.cn/Article/details/gplwnhyuy.sHtML

TS:   nested.flat();
来源：http://www.m.share.fehbvm.com/Article/details/gaxvrbxej.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.blog.hesvh.cn/Article/details/giwbatgpi.sHtML

Go:   // 手写双层循环
来源：http://wap.fehbvm.com/Article/details/ggeobbenc.sHtML

Ruby: nested.flatten
来源：http://read.share.fehbvm.com/Article/details/gyqaboery.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.share.zdbjq.cn/Article/details/gszzpcygj.sHtML

[D19] 按字段分组
来源：http://wap.zdbjq.cn/Article/details/gtvrqzvtg.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://m.share.hesvh.cn/Article/details/gqticgjoi.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://blog.fehbvm.com/Article/details/gspvvzljt.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.blog.zdbjq.cn/Article/details/gnsldhfvx.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://blog.fehbvm.com/Article/details/gaymuyfcw.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://baike.fehbvm.com/Article/details/gfotopvzq.sHtML

Go:   // 手写 map[string][]T
来源：http://blog.zdbjq.cn/Article/details/gjqaugrkd.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://wap.hesvh.cn/Article/details/goofbckeq.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.share.hesvh.cn/Article/details/gmekcsoyj.sHtML

[D20] 统计每个元素出现次数
来源：http://www.m.share.zdbjq.cn/Article/details/gufjikmlu.sHtML

Py:   Counter(arr)
来源：http://www.share.fehbvm.com/Article/details/gumzqvhxy.sHtML

PHP:  array_count_values($arr);
来源：http://wap.zdbjq.cn/Article/details/gpgxqwhbc.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.fehbvm.com/Article/details/gicamropw.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.hesvh.cn/Article/details/gylhxovel.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.blog.fehbvm.com/Article/details/gdazlizef.sHtML

Go:   // 手写 map[T]int
来源：http://blog.fehbvm.com/Article/details/ghurqzffi.sHtML

Ruby: arr.tally
来源：http://mobile.fehbvm.com/Article/details/gwwzvioox.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://mobile.hesvh.cn/Article/details/gplyvsjlx.sHtML

[D21] 判断是否包含某元素
来源：http://www.m.share.fehbvm.com/Article/details/gdgmjdsva.sHtML

Py:   x in arr
来源：http://mobile.fehbvm.com/Article/details/gexbcmaba.sHtML

PHP:  in_array($x, $arr, true);
来源：http://baike.zdbjq.cn/Article/details/gxrfndlyh.sHtML

JS:   arr.includes(x)
来源：http://www.share.zdbjq.cn/Article/details/gbgcxgqpd.sHtML

TS:   arr.includes(x)
来源：http://www.share.hesvh.cn/Article/details/ggxlfaseu.sHtML

Java: list.contains(x)
来源：http://wap.zdbjq.cn/Article/details/gqjjeogdv.sHtML

Go:   slices.Contains(arr, x)
来源：http://mobile.zdbjq.cn/Article/details/ghkyeroyt.sHtML

Ruby: arr.include?(x)
来源：http://blog.zdbjq.cn/Article/details/godrgsxrp.sHtML

C#:   list.Contains(x)
来源：http://baike.hesvh.cn/Article/details/gjxljlyos.sHtML

[D22] 复制数组（避免共享引用）
来源：http://wap.hesvh.cn/Article/details/gzztqcoir.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://mobile.fehbvm.com/Article/details/gidbmcxkv.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://blog.zdbjq.cn/Article/details/gxttczuzs.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://3g.fehbvm.com/Article/details/gdjtubnsa.sHtML

TS:   [...arr];
来源：http://www.blog.hesvh.cn/Article/details/gdcwkfwjr.sHtML

Java: new ArrayList<>(list);
来源：http://3g.zdbjq.cn/Article/details/gqtrzlafp.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://m.share.fehbvm.com/Article/details/gfnzwndso.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.share.zdbjq.cn/Article/details/gdvmwwvdw.sHtML

C#:   new List<int>(list);
来源：http://mobile.hesvh.cn/Article/details/gcpsmykgg.sHtML

[D23] reduce 累积计算
来源：http://m.share.fehbvm.com/Article/details/goujwcyjp.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://read.share.fehbvm.com/Article/details/gpsodelot.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.blog.zdbjq.cn/Article/details/gwnryirag.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.hesvh.cn/Article/details/gyembxjib.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.zdbjq.cn/Article/details/gziggerrt.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://3g.hesvh.cn/Article/details/gydojxlgc.sHtML

Go:   // 手写循环
来源：http://read.share.fehbvm.com/Article/details/gkptohcjz.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.share.fehbvm.com/Article/details/gwbytdwim.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.m.share.fehbvm.com/Article/details/guzjlarje.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.share.fehbvm.com/Article/details/gcskbwgvl.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.m.share.fehbvm.com/Article/details/gnchkpygh.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://3g.hesvh.cn/Article/details/gdbhtoznx.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://m.share.zdbjq.cn/Article/details/gprvxqugz.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.share.hesvh.cn/Article/details/gpdkockrj.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://baike.zdbjq.cn/Article/details/gkvrolgna.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://read.share.hesvh.cn/Article/details/gvdrerjzf.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://baike.hesvh.cn/Article/details/ghsixoitx.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mobile.zdbjq.cn/Article/details/gnhqpbawp.sHtML

[D25] Set 集合去重与交并差
来源：http://www.m.share.zdbjq.cn/Article/details/gklkkzmrv.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://read.share.fehbvm.com/Article/details/gpkqwctdz.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://read.share.hesvh.cn/Article/details/gspsngafk.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://blog.zdbjq.cn/Article/details/gpscpimgb.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://m.share.fehbvm.com/Article/details/gpjedvhph.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.share.hesvh.cn/Article/details/glpyasthm.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.blog.zdbjq.cn/Article/details/gghlnivzz.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mobile.hesvh.cn/Article/details/gbhukzpej.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://read.share.hesvh.cn/Article/details/gdzpsrshx.sHtML

[D26] 数组转字符串
来源：http://blog.zdbjq.cn/Article/details/gqywyzkzm.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.share.zdbjq.cn/Article/details/gwyyfrmhl.sHtML

PHP:  implode(", ", $arr);
来源：http://www.m.share.hesvh.cn/Article/details/gpvhszgmx.sHtML

JS:   arr.join(", ")
来源：http://www.blog.fehbvm.com/Article/details/gpwlvjjsa.sHtML

TS:   arr.join(", ")
来源：http://wap.hesvh.cn/Article/details/gslacjryo.sHtML

Java: String.join(", ", list)
来源：http://mobile.hesvh.cn/Article/details/gogvxovcp.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.m.share.hesvh.cn/Article/details/ghjbysnhf.sHtML

Ruby: arr.join(", ")
来源：http://m.share.fehbvm.com/Article/details/gbkrhetwv.sHtML

C#:   string.Join(", ", list)
来源：http://3g.hesvh.cn/Article/details/gkcxgtfyl.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gmdzaaxht.sHtML

E. 字符串处理
来源：http://mobile.zdbjq.cn/Article/details/guzxfgrfc.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gvztboqeq.sHtML

[E01] 拼接字符串
来源：http://m.share.zdbjq.cn/Article/details/grsdmlcut.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://read.share.fehbvm.com/Article/details/gyfvcvsqq.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.blog.zdbjq.cn/Article/details/gbhrguvju.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.hesvh.cn/Article/details/gqpdhacol.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.fehbvm.com/Article/details/ghaswbkat.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://read.share.hesvh.cn/Article/details/gndbtggfa.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://read.share.fehbvm.com/Article/details/gsbwzvuys.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://3g.hesvh.cn/Article/details/gdhyzupcs.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://wap.zdbjq.cn/Article/details/gniedfkhf.sHtML

[E02] 重复字符串
来源：http://www.share.hesvh.cn/Article/details/gxsomrodo.sHtML

Py:   "ab" * 3
来源：http://www.blog.fehbvm.com/Article/details/gpaursbsj.sHtML

PHP:  str_repeat("ab", 3);
来源：http://3g.zdbjq.cn/Article/details/gwkdpfnnv.sHtML

JS:   "ab".repeat(3)
来源：http://read.share.fehbvm.com/Article/details/grejgbbxs.sHtML

TS:   "ab".repeat(3)
来源：http://3g.zdbjq.cn/Article/details/giwvktgqv.sHtML

Java: "ab".repeat(3)
来源：http://wap.zdbjq.cn/Article/details/ghewgwlau.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://blog.fehbvm.com/Article/details/gboiiqrwe.sHtML

Ruby: "ab" * 3
来源：http://wap.zdbjq.cn/Article/details/gkycjukwn.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://blog.zdbjq.cn/Article/details/gfsjjtzqv.sHtML

[E03] 截取子串
来源：http://blog.hesvh.cn/Article/details/gtvzftkdm.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://3g.fehbvm.com/Article/details/gamnesiqo.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://3g.hesvh.cn/Article/details/gqqcnxmtc.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://3g.hesvh.cn/Article/details/gjmfwugej.sHtML

TS:   s.slice(1, 4)
来源：http://3g.zdbjq.cn/Article/details/gejrgpsnp.sHtML

Java: s.substring(1, 4)
来源：http://www.blog.hesvh.cn/Article/details/gnwopfxoc.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://3g.hesvh.cn/Article/details/gvonxpsnn.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://wap.hesvh.cn/Article/details/goeoqfudl.sHtML

C#:   s.Substring(1, 3)
来源：http://baike.hesvh.cn/Article/details/gvoebindd.sHtML

[E04] 查找子串位置
来源：http://www.share.hesvh.cn/Article/details/gouvpbziv.sHtML

Py:   s.find("x");  s.index("x")
来源：http://baike.hesvh.cn/Article/details/gfmhrfinp.sHtML

PHP:  strpos($s, "x");
来源：http://mobile.hesvh.cn/Article/details/gavrnjoir.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.m.share.hesvh.cn/Article/details/glaitqczm.sHtML

TS:   s.indexOf("x")
来源：http://wap.zdbjq.cn/Article/details/gbpsvgrcm.sHtML

Java: s.indexOf("x")
来源：http://www.blog.zdbjq.cn/Article/details/gdtqqqibe.sHtML

Go:   strings.Index(s, "x")
来源：http://wap.hesvh.cn/Article/details/gktmwzbzt.sHtML

Ruby: s.index("x")
来源：http://read.share.zdbjq.cn/Article/details/gijmpfxzy.sHtML

C#:   s.IndexOf("x")
来源：http://mobile.fehbvm.com/Article/details/gmvpargxu.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://3g.hesvh.cn/Article/details/guiirolym.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://blog.hesvh.cn/Article/details/ghytqomas.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://3g.zdbjq.cn/Article/details/gffediuus.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.zdbjq.cn/Article/details/gtvtfbyhb.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://read.share.hesvh.cn/Article/details/gtovnyoha.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.zdbjq.cn/Article/details/gqrmyjgtb.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://blog.zdbjq.cn/Article/details/ggmtmysys.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.blog.zdbjq.cn/Article/details/gzebaaujz.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://mobile.zdbjq.cn/Article/details/gevrhamih.sHtML

[E06] 替换子串
来源：http://www.m.share.fehbvm.com/Article/details/gdcpiuuna.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://mobile.hesvh.cn/Article/details/gbamlxurs.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.share.hesvh.cn/Article/details/gukaylvrv.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/gvyhkxfki.sHtML

TS:   s.replaceAll("a", "b")
来源：http://read.share.zdbjq.cn/Article/details/gdfsbcyfb.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.fehbvm.com/Article/details/gyefvzbdn.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://blog.hesvh.cn/Article/details/gkjmdxppc.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.m.share.hesvh.cn/Article/details/gqdngdbnf.sHtML

C#:   s.Replace("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/gnvqllvro.sHtML

[E07] 按分隔符拆分
来源：http://www.share.fehbvm.com/Article/details/gvkjipuou.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://baike.zdbjq.cn/Article/details/gejlfuyus.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://3g.fehbvm.com/Article/details/gjdgbpaxx.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.m.share.zdbjq.cn/Article/details/ghrvfgvpc.sHtML

TS:   s.split(",")
来源：http://m.share.hesvh.cn/Article/details/geigwsyaz.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://wap.hesvh.cn/Article/details/gydjiuafy.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://3g.fehbvm.com/Article/details/gtyaipiva.sHtML

Ruby: s.split(",");  s.split
来源：http://www.share.hesvh.cn/Article/details/guichftxd.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.share.fehbvm.com/Article/details/gfcocgtkw.sHtML

[E08] 数组按分隔符合并
来源：http://www.m.share.zdbjq.cn/Article/details/gphhgjhlw.sHtML

Py:   ",".join(items)
来源：http://www.m.share.hesvh.cn/Article/details/guaamgugc.sHtML

PHP:  implode(",", $items);
来源：http://baike.fehbvm.com/Article/details/gfphmjukg.sHtML

JS:   items.join(",")
来源：http://www.blog.hesvh.cn/Article/details/gglojxqcr.sHtML

TS:   items.join(",")
来源：http://3g.fehbvm.com/Article/details/gjktthkbu.sHtML

Java: String.join(",", items)
来源：http://m.share.zdbjq.cn/Article/details/gggaruqff.sHtML

Go:   strings.Join(items, ",")
来源：http://blog.fehbvm.com/Article/details/grzwdqsbe.sHtML

Ruby: items.join(",")
来源：http://read.share.hesvh.cn/Article/details/gapfwbfwp.sHtML

C#:   string.Join(",", items)
来源：http://blog.fehbvm.com/Article/details/gwkcweczk.sHtML

[E09] 去除所有空白字符
来源：http://www.share.zdbjq.cn/Article/details/gyirjgrkd.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://mobile.fehbvm.com/Article/details/gofpbafhv.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://baike.hesvh.cn/Article/details/gxmbdrshh.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.share.fehbvm.com/Article/details/gxpgdihvr.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.m.share.hesvh.cn/Article/details/gvoszwwnk.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://baike.hesvh.cn/Article/details/ggztmsuqs.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://m.share.hesvh.cn/Article/details/gcfuusoeg.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.share.hesvh.cn/Article/details/gcsbwxfvv.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://m.share.zdbjq.cn/Article/details/gydyoqbgh.sHtML

[E10] 左侧补零 / 定长填充
来源：http://3g.hesvh.cn/Article/details/getudxhgx.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.share.hesvh.cn/Article/details/gayephzwu.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://read.share.zdbjq.cn/Article/details/ghwkanioy.sHtML

JS:   "7".padStart(3, "0")
来源：http://3g.zdbjq.cn/Article/details/gwuaxoedt.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.share.hesvh.cn/Article/details/gajmsfkbi.sHtML

Java: String.format("%03d", 7)
来源：http://baike.fehbvm.com/Article/details/gsydbchgl.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://m.share.fehbvm.com/Article/details/gqqpljomo.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://mobile.fehbvm.com/Article/details/goquyfmfw.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://read.share.zdbjq.cn/Article/details/gmmaefsqr.sHtML

[E11] 反转字符串
来源：http://read.share.fehbvm.com/Article/details/gnmrygcuo.sHtML

Py:   s[::-1]
来源：http://mobile.zdbjq.cn/Article/details/gcwmntmht.sHtML

PHP:  strrev($s);
来源：http://3g.fehbvm.com/Article/details/gecjhrbyh.sHtML

JS:   [...s].reverse().join("")
来源：http://www.m.share.hesvh.cn/Article/details/gtztwkwsd.sHtML

TS:   [...s].reverse().join("")
来源：http://www.share.fehbvm.com/Article/details/goxmynfre.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://3g.fehbvm.com/Article/details/gjqxtgdwp.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://wap.fehbvm.com/Article/details/gurtwhdug.sHtML

Ruby: s.reverse
来源：http://wap.hesvh.cn/Article/details/gmvirxpta.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://blog.zdbjq.cn/Article/details/gajocdyeg.sHtML

[E12] 统计某字符出现次数
来源：http://baike.zdbjq.cn/Article/details/gvnmezmrl.sHtML

Py:   s.count("a")
来源：http://read.share.zdbjq.cn/Article/details/gbbfcopgs.sHtML

PHP:  substr_count($s, "a");
来源：http://read.share.hesvh.cn/Article/details/gbacvylcg.sHtML

JS:   s.split("a").length - 1
来源：http://www.m.share.zdbjq.cn/Article/details/gccjeasag.sHtML

TS:   s.split("a").length - 1
来源：http://baike.hesvh.cn/Article/details/genblpmgd.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.blog.hesvh.cn/Article/details/gswlcrczd.sHtML

Go:   strings.Count(s, "a")
来源：http://mobile.hesvh.cn/Article/details/gcriqkacl.sHtML

Ruby: s.count("a")
来源：http://blog.fehbvm.com/Article/details/gbtnkvadv.sHtML

C#:   s.Count(c => c == 'a')
来源：http://wap.hesvh.cn/Article/details/gfyuhyrbo.sHtML

[E13] 逐字符遍历
来源：http://mobile.zdbjq.cn/Article/details/gngpnvmdx.sHtML


<!-- 参考信息 -->