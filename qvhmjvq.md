代发 wailian999

Go:   arr[0]; arr[0] = 9
来源：http://www.share.fehbvm.com/Article/details/gninwzitz.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.hesvh.cn/Article/details/gudbfemfc.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://3g.fehbvm.com/Article/details/gonysratz.sHtML

[D06] 数组长度
来源：http://wap.hesvh.cn/Article/details/gahvxocvj.sHtML

Py:   len(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gjnzgefoe.sHtML

PHP:  count($arr);
来源：http://m.share.fehbvm.com/Article/details/gltmxvkxd.sHtML

JS:   arr.length
来源：http://baike.hesvh.cn/Article/details/gulcuziyo.sHtML

TS:   arr.length
来源：http://m.share.hesvh.cn/Article/details/gfkoqihzm.sHtML

Java: list.size();
来源：http://baike.zdbjq.cn/Article/details/gkjxgnrpe.sHtML

Go:   len(arr)
来源：http://wap.hesvh.cn/Article/details/gnmaeeymg.sHtML

Ruby: arr.length; arr.size
来源：http://m.share.fehbvm.com/Article/details/ghcekeesi.sHtML

C#:   list.Count;
来源：http://read.share.zdbjq.cn/Article/details/gkrhwadzl.sHtML

[D07] 切片 / 取子数组
来源：http://baike.hesvh.cn/Article/details/gnuhkgqct.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.share.zdbjq.cn/Article/details/ghfohiocv.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.share.hesvh.cn/Article/details/gmxcjdqor.sHtML

JS:   arr.slice(1, 4);
来源：http://www.share.hesvh.cn/Article/details/ggjdgwmqz.sHtML

TS:   arr.slice(1, 4);
来源：http://baike.zdbjq.cn/Article/details/ggtkfvvkg.sHtML

Java: list.subList(1, 4);
来源：http://m.share.fehbvm.com/Article/details/gkbvcplxw.sHtML

Go:   arr[1:4]
来源：http://blog.zdbjq.cn/Article/details/gdbxovdxa.sHtML

Ruby: arr[1, 3]
来源：http://mobile.hesvh.cn/Article/details/gcltyavnh.sHtML

C#:   list.GetRange(1, 3);
来源：http://blog.zdbjq.cn/Article/details/gmaqhpbun.sHtML

[D08] 合并两个数组
来源：http://mobile.fehbvm.com/Article/details/gjabaybwb.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.share.zdbjq.cn/Article/details/gbbgudvsk.sHtML

PHP:  array_merge($a, $b);
来源：http://mobile.zdbjq.cn/Article/details/gnvoagsab.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://mobile.fehbvm.com/Article/details/gznmpzmpk.sHtML

TS:   [...a, ...b];
来源：http://blog.zdbjq.cn/Article/details/gysjomhhi.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.blog.hesvh.cn/Article/details/gywsrsspl.sHtML

Go:   append(a, b...)
来源：http://blog.hesvh.cn/Article/details/gswspddjl.sHtML

Ruby: a + b;  a.concat(b)
来源：http://read.share.fehbvm.com/Article/details/gomlglgmh.sHtML

C#:   a.Concat(b).ToList()
来源：http://wap.fehbvm.com/Article/details/gvoqeldoz.sHtML

[D09] 排序（升序）
来源：http://baike.hesvh.cn/Article/details/gmgyrdihp.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.zdbjq.cn/Article/details/gjzjdzkng.sHtML

PHP:  sort($arr);
来源：http://blog.zdbjq.cn/Article/details/gtlmencsg.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.blog.fehbvm.com/Article/details/gvleymptd.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://read.share.fehbvm.com/Article/details/gxuppeajb.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://blog.zdbjq.cn/Article/details/ggcorfrcq.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://m.share.fehbvm.com/Article/details/gfqjltwya.sHtML

Ruby: arr.sort
来源：http://mobile.zdbjq.cn/Article/details/gwwksffdu.sHtML

C#:   list.Sort();
来源：http://blog.fehbvm.com/Article/details/glnruizvb.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://m.share.zdbjq.cn/Article/details/gtgujovwv.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mobile.fehbvm.com/Article/details/gayyasfow.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.hesvh.cn/Article/details/guxhrdzdm.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.zdbjq.cn/Article/details/gxdmntmfo.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.zdbjq.cn/Article/details/genuhnuma.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://blog.hesvh.cn/Article/details/gmzqbtcha.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.m.share.hesvh.cn/Article/details/gwxdvqzdp.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://baike.fehbvm.com/Article/details/glknpkiyv.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.share.zdbjq.cn/Article/details/grteuzfdr.sHtML

[D11] 反转数组
来源：http://www.share.hesvh.cn/Article/details/gsadvalgh.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://baike.hesvh.cn/Article/details/gblcouskj.sHtML

PHP:  array_reverse($arr);
来源：http://wap.hesvh.cn/Article/details/gbptjkrud.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://blog.fehbvm.com/Article/details/gyutrfjdw.sHtML

TS:   [...arr].reverse();
来源：http://www.blog.fehbvm.com/Article/details/gblxfnsol.sHtML

Java: Collections.reverse(list);
来源：http://mobile.zdbjq.cn/Article/details/gsfqpnzuo.sHtML

Go:   slices.Reverse(arr)
来源：http://blog.zdbjq.cn/Article/details/gifiwaadu.sHtML

Ruby: arr.reverse
来源：http://3g.fehbvm.com/Article/details/gklwwvxkt.sHtML

C#:   list.Reverse();
来源：http://read.share.fehbvm.com/Article/details/glxfnhebq.sHtML

[D12] 查找元素下标
来源：http://m.share.fehbvm.com/Article/details/gkwhtxauu.sHtML

Py:   arr.index(x);  x in arr
来源：http://wap.hesvh.cn/Article/details/gsxfwgzzc.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.m.share.fehbvm.com/Article/details/ghtgtxsil.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.fehbvm.com/Article/details/gxnqbepko.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.hesvh.cn/Article/details/gmkwpihlp.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://blog.zdbjq.cn/Article/details/gvwqvymqh.sHtML

Go:   slices.Index(arr, x)
来源：http://mobile.hesvh.cn/Article/details/gvtgrsivp.sHtML

Ruby: arr.index(x)
来源：http://blog.zdbjq.cn/Article/details/gwovemtex.sHtML

C#:   list.IndexOf(x);
来源：http://wap.zdbjq.cn/Article/details/ggkcwsoxc.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.m.share.zdbjq.cn/Article/details/gcjsbgrtx.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://m.share.fehbvm.com/Article/details/guteuqars.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://baike.hesvh.cn/Article/details/gmypbrsfu.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.share.zdbjq.cn/Article/details/gonjhkaye.sHtML

TS:   arr.filter(x => x > 3)
来源：http://baike.hesvh.cn/Article/details/gvfininib.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.blog.fehbvm.com/Article/details/gcdtxcbgo.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://3g.zdbjq.cn/Article/details/gdrwnavue.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.share.fehbvm.com/Article/details/ghkjipnji.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://baike.hesvh.cn/Article/details/gazwmneii.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.m.share.hesvh.cn/Article/details/gaewyqumb.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wap.zdbjq.cn/Article/details/gakilggxt.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.blog.hesvh.cn/Article/details/gkkrobtnd.sHtML

JS:   arr.map(x => x * 2)
来源：http://baike.fehbvm.com/Article/details/gxwnjealf.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gxodprpmz.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.m.share.fehbvm.com/Article/details/gpdgqaeic.sHtML

Go:   // 手写循环
来源：http://www.blog.zdbjq.cn/Article/details/gnrvidsjn.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://m.share.zdbjq.cn/Article/details/gzwmivcyw.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://baike.fehbvm.com/Article/details/gwwbhhant.sHtML

[D15] 去重
来源：http://m.share.fehbvm.com/Article/details/gahlouytm.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://m.share.hesvh.cn/Article/details/gmrenmbhx.sHtML

PHP:  array_unique($arr);
来源：http://wap.hesvh.cn/Article/details/gthrrcgjf.sHtML

JS:   [...new Set(arr)]
来源：http://m.share.hesvh.cn/Article/details/gtpqsrupn.sHtML

TS:   [...new Set(arr)]
来源：http://mobile.zdbjq.cn/Article/details/gfxadfxej.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wap.zdbjq.cn/Article/details/gipaomlmb.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://mobile.zdbjq.cn/Article/details/gsytcyxnk.sHtML

Ruby: arr.uniq
来源：http://blog.fehbvm.com/Article/details/giekgnsrv.sHtML

C#:   list.Distinct().ToList()
来源：http://m.share.hesvh.cn/Article/details/ggymhmmkl.sHtML

[D16] 求和与平均值
来源：http://baike.zdbjq.cn/Article/details/gntnpucvc.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://3g.fehbvm.com/Article/details/gvgausolb.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wap.fehbvm.com/Article/details/gzohrpxlm.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.zdbjq.cn/Article/details/gogrysckp.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.zdbjq.cn/Article/details/gqjrfyjzn.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.share.hesvh.cn/Article/details/gezonahby.sHtML

Go:   // 手写循环累加
来源：http://m.share.hesvh.cn/Article/details/gboaleehn.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.blog.zdbjq.cn/Article/details/gideylqgd.sHtML

C#:   list.Sum();  list.Average()
来源：http://3g.zdbjq.cn/Article/details/gkpxoxoqv.sHtML

[D17] 最大值与最小值
来源：http://baike.fehbvm.com/Article/details/glmxtripi.sHtML

Py:   max(arr);  min(arr)
来源：http://read.share.fehbvm.com/Article/details/gbaamajyc.sHtML

PHP:  max($arr);  min($arr);
来源：http://blog.zdbjq.cn/Article/details/goysfsyim.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://3g.fehbvm.com/Article/details/gfehbfxcl.sHtML

TS:   Math.max(...arr);
来源：http://baike.fehbvm.com/Article/details/gmqqimidy.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://3g.fehbvm.com/Article/details/gsdfqusyp.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.share.hesvh.cn/Article/details/gzhuvxaga.sHtML

Ruby: arr.max;  arr.min
来源：http://baike.fehbvm.com/Article/details/gqzfmektm.sHtML

C#:   list.Max();  list.Min()
来源：http://baike.zdbjq.cn/Article/details/gpbxkrphx.sHtML

[D18] 扁平化嵌套数组
来源：http://www.m.share.hesvh.cn/Article/details/gcqfgzjes.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.blog.fehbvm.com/Article/details/gtzpvrvti.sHtML

PHP:  array_merge(...$nested);
来源：http://3g.zdbjq.cn/Article/details/gxtfscbgo.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mobile.fehbvm.com/Article/details/gjrqvasbr.sHtML

TS:   nested.flat();
来源：http://www.m.share.fehbvm.com/Article/details/gkybhjgyl.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://3g.fehbvm.com/Article/details/ggotqwzxe.sHtML

Go:   // 手写双层循环
来源：http://m.share.fehbvm.com/Article/details/ggavxoekp.sHtML

Ruby: nested.flatten
来源：http://blog.fehbvm.com/Article/details/gqfodsjfu.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.share.hesvh.cn/Article/details/gzzujflmn.sHtML

[D19] 按字段分组
来源：http://mobile.zdbjq.cn/Article/details/gogxijzrn.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.m.share.hesvh.cn/Article/details/gywddsjjk.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://baike.fehbvm.com/Article/details/gyezckmfr.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://blog.hesvh.cn/Article/details/gcetbuwch.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.share.fehbvm.com/Article/details/gtpdiyjaa.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.share.hesvh.cn/Article/details/galbdzbrs.sHtML

Go:   // 手写 map[string][]T
来源：http://www.share.hesvh.cn/Article/details/gxqkbycpz.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://baike.zdbjq.cn/Article/details/gnrwrzfef.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://blog.hesvh.cn/Article/details/gzczwlxzf.sHtML

[D20] 统计每个元素出现次数
来源：http://wap.zdbjq.cn/Article/details/gqksjsncv.sHtML

Py:   Counter(arr)
来源：http://baike.fehbvm.com/Article/details/ghaezznzn.sHtML

PHP:  array_count_values($arr);
来源：http://mobile.zdbjq.cn/Article/details/gofhdwugu.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.hesvh.cn/Article/details/gtwyrgdru.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.hesvh.cn/Article/details/gwrxkfmey.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mobile.fehbvm.com/Article/details/gpcthrhtc.sHtML

Go:   // 手写 map[T]int
来源：http://mobile.zdbjq.cn/Article/details/gowthryvo.sHtML

Ruby: arr.tally
来源：http://www.share.hesvh.cn/Article/details/guimdmffd.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://read.share.zdbjq.cn/Article/details/gbxacocym.sHtML

[D21] 判断是否包含某元素
来源：http://read.share.zdbjq.cn/Article/details/glbephpxo.sHtML

Py:   x in arr
来源：http://www.m.share.hesvh.cn/Article/details/gyxckcpha.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.m.share.fehbvm.com/Article/details/gabifyfpl.sHtML

JS:   arr.includes(x)
来源：http://m.share.fehbvm.com/Article/details/gkydiomob.sHtML

TS:   arr.includes(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gtxepvqwp.sHtML

Java: list.contains(x)
来源：http://baike.hesvh.cn/Article/details/gydbebjux.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/gvnqbjhca.sHtML

Ruby: arr.include?(x)
来源：http://www.m.share.hesvh.cn/Article/details/gbsplqvvt.sHtML

C#:   list.Contains(x)
来源：http://www.blog.zdbjq.cn/Article/details/gkewbchqx.sHtML

[D22] 复制数组（避免共享引用）
来源：http://wap.hesvh.cn/Article/details/gpcjxcofj.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://m.share.fehbvm.com/Article/details/gjnbctenl.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.m.share.zdbjq.cn/Article/details/gkzgimtrd.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wap.hesvh.cn/Article/details/gwoczexqe.sHtML

TS:   [...arr];
来源：http://mobile.fehbvm.com/Article/details/gqgtwowmb.sHtML

Java: new ArrayList<>(list);
来源：http://www.blog.zdbjq.cn/Article/details/gelskqlcc.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://wap.zdbjq.cn/Article/details/gsusmyzzf.sHtML

Ruby: arr.dup;  arr.clone
来源：http://m.share.zdbjq.cn/Article/details/glcmoiasy.sHtML

C#:   new List<int>(list);
来源：http://blog.fehbvm.com/Article/details/gnqmuxfig.sHtML

[D23] reduce 累积计算
来源：http://wap.hesvh.cn/Article/details/gtuiwbfjz.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.share.fehbvm.com/Article/details/grtacduds.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.m.share.hesvh.cn/Article/details/gfsvrotyp.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.zdbjq.cn/Article/details/grgtvejfz.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.hesvh.cn/Article/details/gxtiobdfm.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.share.hesvh.cn/Article/details/gnucwzfgt.sHtML

Go:   // 手写循环
来源：http://baike.zdbjq.cn/Article/details/gykrkaoqc.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://baike.fehbvm.com/Article/details/gwqbmokds.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://3g.fehbvm.com/Article/details/gsnccypnv.sHtML

[D24] 字典 / Map 基本操作
来源：http://read.share.zdbjq.cn/Article/details/glsarzpzd.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mobile.fehbvm.com/Article/details/gomkqytzh.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.share.hesvh.cn/Article/details/gbzywawzr.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wap.fehbvm.com/Article/details/gjoxtpehd.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.share.zdbjq.cn/Article/details/gtovtdrqd.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://mobile.zdbjq.cn/Article/details/gygkohgxj.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.blog.fehbvm.com/Article/details/gfcfgthhe.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.m.share.zdbjq.cn/Article/details/gxlyrhpvu.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://blog.fehbvm.com/Article/details/giupdjqdz.sHtML

[D25] Set 集合去重与交并差
来源：http://wap.fehbvm.com/Article/details/grufwanuy.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://baike.fehbvm.com/Article/details/gduanvkss.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://blog.hesvh.cn/Article/details/guximqxwq.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wap.fehbvm.com/Article/details/gffyomqqj.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://read.share.zdbjq.cn/Article/details/gkxfafjwn.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://mobile.zdbjq.cn/Article/details/gynpydclh.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.m.share.fehbvm.com/Article/details/gvpzyprtc.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://read.share.fehbvm.com/Article/details/ghvpszded.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mobile.hesvh.cn/Article/details/glpsvgxcm.sHtML

[D26] 数组转字符串
来源：http://blog.zdbjq.cn/Article/details/gcdbfvqwx.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.blog.zdbjq.cn/Article/details/gilebfvue.sHtML

PHP:  implode(", ", $arr);
来源：http://mobile.hesvh.cn/Article/details/gbthnqlro.sHtML

JS:   arr.join(", ")
来源：http://read.share.fehbvm.com/Article/details/gcbbjromq.sHtML

TS:   arr.join(", ")
来源：http://www.m.share.hesvh.cn/Article/details/grjekgtpt.sHtML

Java: String.join(", ", list)
来源：http://read.share.zdbjq.cn/Article/details/gslxrmzeh.sHtML

Go:   strings.Join(strs, ", ")
来源：http://blog.fehbvm.com/Article/details/geipxwvkp.sHtML

Ruby: arr.join(", ")
来源：http://m.share.zdbjq.cn/Article/details/glnwxcepr.sHtML

C#:   string.Join(", ", list)
来源：http://wap.zdbjq.cn/Article/details/gurscoicd.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gvvhwjofk.sHtML

E. 字符串处理
来源：http://www.blog.hesvh.cn/Article/details/goxuyntwk.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/ghltqtlub.sHtML

[E01] 拼接字符串
来源：http://www.share.fehbvm.com/Article/details/gkkeqxxtq.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.blog.fehbvm.com/Article/details/gsjjalkik.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://m.share.hesvh.cn/Article/details/gcehikvhx.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.hesvh.cn/Article/details/gfcouqcre.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gozukjbws.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.m.share.fehbvm.com/Article/details/goxoydtus.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://mobile.hesvh.cn/Article/details/gyhvjjlpl.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.share.fehbvm.com/Article/details/govgthiiq.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://wap.hesvh.cn/Article/details/gejzhfnwo.sHtML

[E02] 重复字符串
来源：http://wap.hesvh.cn/Article/details/gfyeyskpr.sHtML

Py:   "ab" * 3
来源：http://mobile.fehbvm.com/Article/details/glcocfjyx.sHtML

PHP:  str_repeat("ab", 3);
来源：http://baike.zdbjq.cn/Article/details/glmlwyegu.sHtML

JS:   "ab".repeat(3)
来源：http://www.share.hesvh.cn/Article/details/gjkqgcpee.sHtML

TS:   "ab".repeat(3)
来源：http://read.share.zdbjq.cn/Article/details/gmvqxnmgh.sHtML

Java: "ab".repeat(3)
来源：http://www.m.share.zdbjq.cn/Article/details/gpvemezfi.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://baike.zdbjq.cn/Article/details/gwzfmhtpn.sHtML

Ruby: "ab" * 3
来源：http://3g.hesvh.cn/Article/details/gxmmysbyy.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://baike.hesvh.cn/Article/details/gclzlpvfd.sHtML

[E03] 截取子串
来源：http://wap.zdbjq.cn/Article/details/gwhhmplsk.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.m.share.zdbjq.cn/Article/details/gmklnulnb.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://m.share.zdbjq.cn/Article/details/gxhvcknen.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://m.share.zdbjq.cn/Article/details/grwljnhka.sHtML

TS:   s.slice(1, 4)
来源：http://www.blog.zdbjq.cn/Article/details/gtxgxkvrp.sHtML

Java: s.substring(1, 4)
来源：http://wap.hesvh.cn/Article/details/ggqdscxrj.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.m.share.zdbjq.cn/Article/details/gnjljbxag.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://3g.fehbvm.com/Article/details/gccmrknof.sHtML

C#:   s.Substring(1, 3)
来源：http://www.share.fehbvm.com/Article/details/gunetxoln.sHtML

[E04] 查找子串位置
来源：http://3g.zdbjq.cn/Article/details/gsgipqeze.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.m.share.hesvh.cn/Article/details/gchtcxtxr.sHtML

PHP:  strpos($s, "x");
来源：http://m.share.zdbjq.cn/Article/details/gdblgsigh.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://3g.hesvh.cn/Article/details/gnuthyqri.sHtML

TS:   s.indexOf("x")
来源：http://m.share.zdbjq.cn/Article/details/gufgqqkqe.sHtML

Java: s.indexOf("x")
来源：http://mobile.hesvh.cn/Article/details/gajxdvrjx.sHtML

Go:   strings.Index(s, "x")
来源：http://www.m.share.zdbjq.cn/Article/details/gnurdbcvf.sHtML

Ruby: s.index("x")
来源：http://read.share.zdbjq.cn/Article/details/gxtlaclch.sHtML

C#:   s.IndexOf("x")
来源：http://www.blog.zdbjq.cn/Article/details/gzjvgktdr.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://blog.zdbjq.cn/Article/details/gnzjhejdu.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.blog.zdbjq.cn/Article/details/guiriznsh.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.share.zdbjq.cn/Article/details/gepwckksr.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.fehbvm.com/Article/details/gwlxzstei.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://mobile.hesvh.cn/Article/details/gzlqgfpof.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.hesvh.cn/Article/details/gwjaukrcn.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://read.share.fehbvm.com/Article/details/gzjdtetpd.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://3g.zdbjq.cn/Article/details/gellovvqo.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://wap.fehbvm.com/Article/details/gjrifnaec.sHtML

[E06] 替换子串
来源：http://wap.hesvh.cn/Article/details/gcjkaezwp.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://read.share.hesvh.cn/Article/details/ggngzphao.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.blog.zdbjq.cn/Article/details/gufjuxjbz.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/ghocxuhsm.sHtML

TS:   s.replaceAll("a", "b")
来源：http://blog.zdbjq.cn/Article/details/grcctgafc.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.fehbvm.com/Article/details/gdirwrhdd.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wap.fehbvm.com/Article/details/grsvopkhn.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://read.share.zdbjq.cn/Article/details/gszexpgsj.sHtML

C#:   s.Replace("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/gstkoypyr.sHtML

[E07] 按分隔符拆分
来源：http://www.m.share.hesvh.cn/Article/details/gavdnkerr.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.blog.hesvh.cn/Article/details/gfvcpzawf.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.blog.zdbjq.cn/Article/details/gwipcowpn.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://mobile.hesvh.cn/Article/details/ghooxcwfs.sHtML

TS:   s.split(",")
来源：http://www.blog.zdbjq.cn/Article/details/glodykoid.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://blog.fehbvm.com/Article/details/goydeihie.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.blog.hesvh.cn/Article/details/gqjqbblnw.sHtML

Ruby: s.split(",");  s.split
来源：http://www.share.zdbjq.cn/Article/details/gtvdspdin.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://mobile.hesvh.cn/Article/details/ggtscwffd.sHtML

[E08] 数组按分隔符合并
来源：http://blog.hesvh.cn/Article/details/gbkshbfwu.sHtML

Py:   ",".join(items)
来源：http://www.blog.fehbvm.com/Article/details/gszgujwsa.sHtML

PHP:  implode(",", $items);
来源：http://read.share.zdbjq.cn/Article/details/gwwujnfmd.sHtML

JS:   items.join(",")
来源：http://blog.zdbjq.cn/Article/details/gturhauzq.sHtML

TS:   items.join(",")
来源：http://www.share.fehbvm.com/Article/details/gzneygvmq.sHtML

Java: String.join(",", items)
来源：http://blog.hesvh.cn/Article/details/gqmfzfwwt.sHtML

Go:   strings.Join(items, ",")
来源：http://mobile.hesvh.cn/Article/details/gfqniddvb.sHtML

Ruby: items.join(",")
来源：http://m.share.fehbvm.com/Article/details/gkmgxotki.sHtML

C#:   string.Join(",", items)
来源：http://mobile.fehbvm.com/Article/details/gsvfqesbn.sHtML

[E09] 去除所有空白字符
来源：http://baike.fehbvm.com/Article/details/gpmqauyta.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://read.share.zdbjq.cn/Article/details/gdsxsmbfc.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://3g.hesvh.cn/Article/details/gslnclpxg.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://wap.hesvh.cn/Article/details/gmpdrfemb.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://wap.fehbvm.com/Article/details/gbpmvbllk.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://baike.zdbjq.cn/Article/details/gdfjygovo.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.m.share.hesvh.cn/Article/details/gjobddezc.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.blog.zdbjq.cn/Article/details/ghblbzkwt.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://3g.zdbjq.cn/Article/details/guweifjzo.sHtML

[E10] 左侧补零 / 定长填充
来源：http://blog.fehbvm.com/Article/details/ghleolfzc.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://blog.fehbvm.com/Article/details/gggkkrxrz.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.share.hesvh.cn/Article/details/gureigzqd.sHtML

JS:   "7".padStart(3, "0")
来源：http://mobile.fehbvm.com/Article/details/gzrzysxga.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.m.share.fehbvm.com/Article/details/gyjzwffxe.sHtML

Java: String.format("%03d", 7)
来源：http://baike.hesvh.cn/Article/details/gecbiuopg.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.m.share.fehbvm.com/Article/details/gpwlcsksq.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.share.fehbvm.com/Article/details/gzeqwiiza.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.blog.fehbvm.com/Article/details/gzrtqhqnc.sHtML

[E11] 反转字符串
来源：http://read.share.hesvh.cn/Article/details/gjhaufwtx.sHtML

Py:   s[::-1]
来源：http://www.m.share.zdbjq.cn/Article/details/gzuaqqorv.sHtML

PHP:  strrev($s);
来源：http://read.share.fehbvm.com/Article/details/gsxxljfvb.sHtML

JS:   [...s].reverse().join("")
来源：http://3g.zdbjq.cn/Article/details/gedxwwatx.sHtML

TS:   [...s].reverse().join("")
来源：http://mobile.hesvh.cn/Article/details/gvzliufva.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://3g.hesvh.cn/Article/details/gnhozykrm.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://m.share.hesvh.cn/Article/details/gjosmcnhc.sHtML

Ruby: s.reverse
来源：http://baike.fehbvm.com/Article/details/gbgqjwjoa.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.blog.fehbvm.com/Article/details/gffypinvp.sHtML

[E12] 统计某字符出现次数
来源：http://3g.zdbjq.cn/Article/details/gkpczefqd.sHtML

Py:   s.count("a")
来源：http://baike.fehbvm.com/Article/details/glcmlfsts.sHtML

PHP:  substr_count($s, "a");
来源：http://wap.fehbvm.com/Article/details/gtgrygzbb.sHtML

JS:   s.split("a").length - 1
来源：http://mobile.zdbjq.cn/Article/details/gofbpxfxm.sHtML

TS:   s.split("a").length - 1
来源：http://baike.hesvh.cn/Article/details/grsaulvpr.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.m.share.zdbjq.cn/Article/details/grkypcrnr.sHtML


<!-- 参考信息 -->