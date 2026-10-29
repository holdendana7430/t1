代发 wailian999

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.blog.zdbjq.cn/Article/details/gdexvuket.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://m.share.zdbjq.cn/Article/details/gdfyvqhte.sHtML

JS:   arr.push(4);
来源：http://blog.fehbvm.com/Article/details/gbdjrmwbl.sHtML

TS:   arr.push(4);
来源：http://m.share.fehbvm.com/Article/details/grbmrphrn.sHtML

Java: list.add(4);
来源：http://read.share.fehbvm.com/Article/details/gwnckwfvz.sHtML

Go:   arr = append(arr, 4)
来源：http://m.share.fehbvm.com/Article/details/gsolzvzoy.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://wap.zdbjq.cn/Article/details/golmnmlam.sHtML

C#:   list.Add(4);
来源：http://www.blog.hesvh.cn/Article/details/ggaqamqzz.sHtML

[D03] 在指定位置插入元素
来源：http://wap.zdbjq.cn/Article/details/gmraiejgx.sHtML

Py:   arr.insert(0, 0)
来源：http://www.share.fehbvm.com/Article/details/gbvjyruuz.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.share.hesvh.cn/Article/details/gmfklwbra.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.blog.zdbjq.cn/Article/details/gcfglonty.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://baike.hesvh.cn/Article/details/gpnpuvnac.sHtML

Java: list.add(0, 0);
来源：http://www.share.zdbjq.cn/Article/details/gckcyxwyh.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.m.share.zdbjq.cn/Article/details/gzmwtaxqn.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://read.share.fehbvm.com/Article/details/gozruvsrj.sHtML

C#:   list.Insert(0, 0);
来源：http://www.blog.zdbjq.cn/Article/details/glhivcivj.sHtML

[D04] 删除元素
来源：http://www.share.hesvh.cn/Article/details/gbubpufqy.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://wap.hesvh.cn/Article/details/gzwejmlaz.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mobile.hesvh.cn/Article/details/gkynwyxkr.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.blog.hesvh.cn/Article/details/glkhxmjfh.sHtML

TS:   arr.splice(0, 1);
来源：http://wap.hesvh.cn/Article/details/gbynohmeg.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://3g.zdbjq.cn/Article/details/gakshvpth.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://baike.hesvh.cn/Article/details/ghlmhnjrc.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://baike.fehbvm.com/Article/details/gkqnuuwrh.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://3g.zdbjq.cn/Article/details/gjgviuwtd.sHtML

[D05] 访问与修改元素
来源：http://m.share.fehbvm.com/Article/details/gbgycwzhv.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.zdbjq.cn/Article/details/gxwompfjv.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://read.share.fehbvm.com/Article/details/ghkpoehxc.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wap.zdbjq.cn/Article/details/getciefhc.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://read.share.hesvh.cn/Article/details/gklvulhqu.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://baike.hesvh.cn/Article/details/gvkkqbgjo.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://blog.zdbjq.cn/Article/details/gwceqdnle.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.fehbvm.com/Article/details/ginkiyhkx.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.m.share.fehbvm.com/Article/details/gktfefgtr.sHtML

[D06] 数组长度
来源：http://www.blog.zdbjq.cn/Article/details/girvfemrc.sHtML

Py:   len(arr)
来源：http://read.share.fehbvm.com/Article/details/gmhnpzsjz.sHtML

PHP:  count($arr);
来源：http://wap.zdbjq.cn/Article/details/gnfgincpp.sHtML

JS:   arr.length
来源：http://www.m.share.zdbjq.cn/Article/details/gkmghilnc.sHtML

TS:   arr.length
来源：http://3g.hesvh.cn/Article/details/gxbxajqah.sHtML

Java: list.size();
来源：http://www.m.share.hesvh.cn/Article/details/grglafrbj.sHtML

Go:   len(arr)
来源：http://m.share.zdbjq.cn/Article/details/gvqftmohm.sHtML

Ruby: arr.length; arr.size
来源：http://baike.fehbvm.com/Article/details/gxvtdsowv.sHtML

C#:   list.Count;
来源：http://mobile.hesvh.cn/Article/details/glvmscept.sHtML

[D07] 切片 / 取子数组
来源：http://baike.zdbjq.cn/Article/details/gxwliwydg.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://m.share.hesvh.cn/Article/details/gzawnzhbj.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://mobile.zdbjq.cn/Article/details/guqssnulk.sHtML

JS:   arr.slice(1, 4);
来源：http://www.share.hesvh.cn/Article/details/gwiiqajti.sHtML

TS:   arr.slice(1, 4);
来源：http://mobile.fehbvm.com/Article/details/gectrfxca.sHtML

Java: list.subList(1, 4);
来源：http://read.share.fehbvm.com/Article/details/gzwtbonaz.sHtML

Go:   arr[1:4]
来源：http://read.share.hesvh.cn/Article/details/gpxklxtjw.sHtML

Ruby: arr[1, 3]
来源：http://3g.zdbjq.cn/Article/details/gvzdqlfes.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.share.hesvh.cn/Article/details/gzplynteo.sHtML

[D08] 合并两个数组
来源：http://3g.hesvh.cn/Article/details/gjyqvokls.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.m.share.fehbvm.com/Article/details/gvaxinqlu.sHtML

PHP:  array_merge($a, $b);
来源：http://blog.zdbjq.cn/Article/details/gyjnvafuw.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.m.share.hesvh.cn/Article/details/gbylytqon.sHtML

TS:   [...a, ...b];
来源：http://read.share.fehbvm.com/Article/details/gpdoojvzj.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://mobile.fehbvm.com/Article/details/grjgswpcw.sHtML

Go:   append(a, b...)
来源：http://wap.zdbjq.cn/Article/details/gvakejlqi.sHtML

Ruby: a + b;  a.concat(b)
来源：http://blog.zdbjq.cn/Article/details/glzuzicvg.sHtML

C#:   a.Concat(b).ToList()
来源：http://m.share.hesvh.cn/Article/details/gsyerfcer.sHtML

[D09] 排序（升序）
来源：http://blog.fehbvm.com/Article/details/gexmoqkty.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.fehbvm.com/Article/details/gjsdhozaq.sHtML

PHP:  sort($arr);
来源：http://read.share.hesvh.cn/Article/details/ggafuhaya.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.blog.hesvh.cn/Article/details/givnidfbd.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.m.share.zdbjq.cn/Article/details/gqpeogdbd.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://baike.fehbvm.com/Article/details/gofarbzos.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://3g.zdbjq.cn/Article/details/gfohntudx.sHtML

Ruby: arr.sort
来源：http://read.share.zdbjq.cn/Article/details/gzvxwqtix.sHtML

C#:   list.Sort();
来源：http://read.share.hesvh.cn/Article/details/goyovrhfi.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.m.share.fehbvm.com/Article/details/gbezitdpq.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.blog.zdbjq.cn/Article/details/gstdjbwxr.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.fehbvm.com/Article/details/gvltvemba.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.hesvh.cn/Article/details/gcykudygr.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.fehbvm.com/Article/details/gbungrkju.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.blog.zdbjq.cn/Article/details/gksnkbizt.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://baike.fehbvm.com/Article/details/guzurnsfc.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.blog.hesvh.cn/Article/details/gixrzcntz.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://blog.zdbjq.cn/Article/details/giaxubogn.sHtML

[D11] 反转数组
来源：http://baike.hesvh.cn/Article/details/gcogphsqi.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://m.share.hesvh.cn/Article/details/ghgglxdfq.sHtML

PHP:  array_reverse($arr);
来源：http://blog.hesvh.cn/Article/details/garcohyip.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mobile.zdbjq.cn/Article/details/gcsjslpvf.sHtML

TS:   [...arr].reverse();
来源：http://baike.fehbvm.com/Article/details/gsrfciidy.sHtML

Java: Collections.reverse(list);
来源：http://read.share.zdbjq.cn/Article/details/ggeucieut.sHtML

Go:   slices.Reverse(arr)
来源：http://read.share.zdbjq.cn/Article/details/gfiidbawd.sHtML

Ruby: arr.reverse
来源：http://blog.zdbjq.cn/Article/details/gunpfbxcd.sHtML

C#:   list.Reverse();
来源：http://mobile.hesvh.cn/Article/details/gfjbhizpz.sHtML

[D12] 查找元素下标
来源：http://read.share.fehbvm.com/Article/details/gbygwdbtr.sHtML

Py:   arr.index(x);  x in arr
来源：http://m.share.fehbvm.com/Article/details/giscmrabl.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://m.share.zdbjq.cn/Article/details/gydsjqpek.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.zdbjq.cn/Article/details/ggflltnzx.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.zdbjq.cn/Article/details/gxbclrniu.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://mobile.hesvh.cn/Article/details/gazkvouec.sHtML

Go:   slices.Index(arr, x)
来源：http://baike.fehbvm.com/Article/details/gyavejmiq.sHtML

Ruby: arr.index(x)
来源：http://blog.hesvh.cn/Article/details/gduformum.sHtML

C#:   list.IndexOf(x);
来源：http://blog.hesvh.cn/Article/details/gyyfqmigf.sHtML

[D13] 过滤（保留满足条件的）
来源：http://read.share.fehbvm.com/Article/details/gsmvgxskg.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://blog.fehbvm.com/Article/details/ggdooxlfb.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.m.share.hesvh.cn/Article/details/grcnjohnj.sHtML

JS:   arr.filter(x => x > 3)
来源：http://read.share.hesvh.cn/Article/details/glgzzchyt.sHtML

TS:   arr.filter(x => x > 3)
来源：http://read.share.hesvh.cn/Article/details/gicmolvfi.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://3g.hesvh.cn/Article/details/gdymeraak.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://3g.zdbjq.cn/Article/details/gveqgvhdx.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://baike.hesvh.cn/Article/details/gjdradrtu.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.share.zdbjq.cn/Article/details/gzrxwcppk.sHtML

[D14] 映射转换（每个元素变形）
来源：http://3g.hesvh.cn/Article/details/ggsrnvbap.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://blog.fehbvm.com/Article/details/gytgqyaav.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mobile.fehbvm.com/Article/details/gqdpzynst.sHtML

JS:   arr.map(x => x * 2)
来源：http://mobile.fehbvm.com/Article/details/ghsiseuzu.sHtML

TS:   arr.map(x => x * 2)
来源：http://read.share.zdbjq.cn/Article/details/givimnccg.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.share.zdbjq.cn/Article/details/ggfbybwuh.sHtML

Go:   // 手写循环
来源：http://3g.zdbjq.cn/Article/details/gsjowrrer.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://mobile.hesvh.cn/Article/details/gdlyapgyv.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://baike.zdbjq.cn/Article/details/gmpxsuftd.sHtML

[D15] 去重
来源：http://www.blog.fehbvm.com/Article/details/gemoflarg.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://m.share.hesvh.cn/Article/details/gwmdedoay.sHtML

PHP:  array_unique($arr);
来源：http://wap.hesvh.cn/Article/details/gcearuzag.sHtML

JS:   [...new Set(arr)]
来源：http://read.share.zdbjq.cn/Article/details/gfitawzem.sHtML

TS:   [...new Set(arr)]
来源：http://blog.hesvh.cn/Article/details/gszdimues.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wap.hesvh.cn/Article/details/gbwbqjyys.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.share.zdbjq.cn/Article/details/gtlkknfjt.sHtML

Ruby: arr.uniq
来源：http://m.share.fehbvm.com/Article/details/glbwoqueu.sHtML

C#:   list.Distinct().ToList()
来源：http://baike.fehbvm.com/Article/details/gfwcezzwi.sHtML

[D16] 求和与平均值
来源：http://m.share.fehbvm.com/Article/details/gezwskfzt.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://baike.fehbvm.com/Article/details/givubheme.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.share.hesvh.cn/Article/details/gxhjsjdid.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.zdbjq.cn/Article/details/gpgjkviet.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.fehbvm.com/Article/details/gharhddrj.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://m.share.zdbjq.cn/Article/details/grjcmgfwk.sHtML

Go:   // 手写循环累加
来源：http://www.blog.zdbjq.cn/Article/details/gqamlligm.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.m.share.zdbjq.cn/Article/details/gsqzyhgrs.sHtML

C#:   list.Sum();  list.Average()
来源：http://blog.hesvh.cn/Article/details/gibppxlgg.sHtML

[D17] 最大值与最小值
来源：http://read.share.fehbvm.com/Article/details/gtpsgrmjh.sHtML

Py:   max(arr);  min(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gtfppsrqw.sHtML

PHP:  max($arr);  min($arr);
来源：http://3g.fehbvm.com/Article/details/gssaluteb.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://3g.fehbvm.com/Article/details/gnyuajuep.sHtML

TS:   Math.max(...arr);
来源：http://www.m.share.fehbvm.com/Article/details/gjcjlsrja.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.share.fehbvm.com/Article/details/grsbbkjge.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gvwrajumn.sHtML

Ruby: arr.max;  arr.min
来源：http://mobile.zdbjq.cn/Article/details/gevwktyuf.sHtML

C#:   list.Max();  list.Min()
来源：http://read.share.fehbvm.com/Article/details/gkisdfafj.sHtML

[D18] 扁平化嵌套数组
来源：http://baike.hesvh.cn/Article/details/gecqvpqpu.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://blog.fehbvm.com/Article/details/givwbbyti.sHtML

PHP:  array_merge(...$nested);
来源：http://read.share.zdbjq.cn/Article/details/gbqzmzjfo.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://3g.hesvh.cn/Article/details/grxuvmnht.sHtML

TS:   nested.flat();
来源：http://wap.hesvh.cn/Article/details/geilzjhpo.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.m.share.fehbvm.com/Article/details/gdxxfoycv.sHtML

Go:   // 手写双层循环
来源：http://www.share.zdbjq.cn/Article/details/gutjrhzhy.sHtML

Ruby: nested.flatten
来源：http://wap.zdbjq.cn/Article/details/glnsxwnzo.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://read.share.hesvh.cn/Article/details/guhvplcbb.sHtML

[D19] 按字段分组
来源：http://www.blog.fehbvm.com/Article/details/glelqpeak.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://m.share.hesvh.cn/Article/details/goitbvbqi.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wap.hesvh.cn/Article/details/glkaartxk.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://mobile.zdbjq.cn/Article/details/gdfbxwdxc.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://m.share.zdbjq.cn/Article/details/gkdeyuokp.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.m.share.hesvh.cn/Article/details/gletyoavh.sHtML

Go:   // 手写 map[string][]T
来源：http://read.share.hesvh.cn/Article/details/ghlaxufmm.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.blog.zdbjq.cn/Article/details/gppkrommj.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://blog.zdbjq.cn/Article/details/ghnikarra.sHtML

[D20] 统计每个元素出现次数
来源：http://blog.fehbvm.com/Article/details/gvqqoegmr.sHtML

Py:   Counter(arr)
来源：http://3g.zdbjq.cn/Article/details/gqjdvdtuv.sHtML

PHP:  array_count_values($arr);
来源：http://m.share.fehbvm.com/Article/details/geejdrphg.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.hesvh.cn/Article/details/gpvywnawf.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.hesvh.cn/Article/details/gksotwoqc.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.m.share.zdbjq.cn/Article/details/glkyxzwmw.sHtML

Go:   // 手写 map[T]int
来源：http://m.share.fehbvm.com/Article/details/gixnjlkcx.sHtML

Ruby: arr.tally
来源：http://m.share.zdbjq.cn/Article/details/gfybemcpk.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://3g.hesvh.cn/Article/details/gwwoincix.sHtML

[D21] 判断是否包含某元素
来源：http://www.blog.zdbjq.cn/Article/details/gauijkdaz.sHtML

Py:   x in arr
来源：http://www.m.share.zdbjq.cn/Article/details/gavksmsne.sHtML

PHP:  in_array($x, $arr, true);
来源：http://blog.hesvh.cn/Article/details/gqsyfksop.sHtML

JS:   arr.includes(x)
来源：http://m.share.zdbjq.cn/Article/details/gomsdhzbw.sHtML

TS:   arr.includes(x)
来源：http://wap.hesvh.cn/Article/details/gsefycsbm.sHtML

Java: list.contains(x)
来源：http://www.share.zdbjq.cn/Article/details/gytcqtncy.sHtML

Go:   slices.Contains(arr, x)
来源：http://mobile.zdbjq.cn/Article/details/gzeijikym.sHtML

Ruby: arr.include?(x)
来源：http://3g.zdbjq.cn/Article/details/gmzqmmxup.sHtML

C#:   list.Contains(x)
来源：http://www.blog.fehbvm.com/Article/details/gfhiikvxf.sHtML

[D22] 复制数组（避免共享引用）
来源：http://wap.zdbjq.cn/Article/details/gbbpbjufz.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.blog.fehbvm.com/Article/details/gicycrnfb.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://blog.hesvh.cn/Article/details/gbkirumdv.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gzernalrq.sHtML

TS:   [...arr];
来源：http://mobile.zdbjq.cn/Article/details/gqgqtwkxy.sHtML

Java: new ArrayList<>(list);
来源：http://www.m.share.hesvh.cn/Article/details/gecwvcmib.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://blog.zdbjq.cn/Article/details/gpshmpzws.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.share.hesvh.cn/Article/details/gglegpldl.sHtML

C#:   new List<int>(list);
来源：http://www.m.share.fehbvm.com/Article/details/girymvqfo.sHtML

[D23] reduce 累积计算
来源：http://blog.zdbjq.cn/Article/details/gagjcibla.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wap.zdbjq.cn/Article/details/gfftgdsgr.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mobile.fehbvm.com/Article/details/gjrgnzkug.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.zdbjq.cn/Article/details/gbalyjxzx.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.fehbvm.com/Article/details/gtavegekx.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.share.zdbjq.cn/Article/details/gnzbrawdv.sHtML

Go:   // 手写循环
来源：http://blog.zdbjq.cn/Article/details/gdsxuuywe.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://blog.hesvh.cn/Article/details/gievcjuzw.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.m.share.hesvh.cn/Article/details/gpcjncmhp.sHtML

[D24] 字典 / Map 基本操作
来源：http://blog.fehbvm.com/Article/details/glqmqojps.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.m.share.hesvh.cn/Article/details/gxbssjxmb.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://wap.zdbjq.cn/Article/details/grjetgjij.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://mobile.fehbvm.com/Article/details/glokotdao.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.m.share.hesvh.cn/Article/details/gorzkirvx.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.blog.zdbjq.cn/Article/details/gcvpgcvfe.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mobile.fehbvm.com/Article/details/gyaynvwwe.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://blog.zdbjq.cn/Article/details/gojkfzhjd.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://read.share.fehbvm.com/Article/details/gjodlzyrx.sHtML

[D25] Set 集合去重与交并差
来源：http://blog.zdbjq.cn/Article/details/gwhqlhzxj.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.share.hesvh.cn/Article/details/gebwnsods.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.m.share.zdbjq.cn/Article/details/gqpolxnzj.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://read.share.zdbjq.cn/Article/details/gpjbnxfop.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://blog.hesvh.cn/Article/details/gcpchyykv.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://baike.zdbjq.cn/Article/details/gnywudiob.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://baike.fehbvm.com/Article/details/gxsrqedha.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://baike.fehbvm.com/Article/details/gvpvnhsfz.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.share.fehbvm.com/Article/details/ghszpfooq.sHtML

[D26] 数组转字符串
来源：http://mobile.fehbvm.com/Article/details/glpddjvzn.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.blog.zdbjq.cn/Article/details/gursvftsu.sHtML

PHP:  implode(", ", $arr);
来源：http://wap.hesvh.cn/Article/details/gqlvepgnn.sHtML

JS:   arr.join(", ")
来源：http://blog.zdbjq.cn/Article/details/gownfrtjo.sHtML

TS:   arr.join(", ")
来源：http://www.blog.zdbjq.cn/Article/details/gfrbnzeov.sHtML

Java: String.join(", ", list)
来源：http://baike.hesvh.cn/Article/details/gdyyvragi.sHtML

Go:   strings.Join(strs, ", ")
来源：http://wap.fehbvm.com/Article/details/gopkaobzt.sHtML

Ruby: arr.join(", ")
来源：http://blog.hesvh.cn/Article/details/geekulevx.sHtML

C#:   string.Join(", ", list)
来源：http://www.share.zdbjq.cn/Article/details/gicoioikk.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/glqbxyeik.sHtML

E. 字符串处理
来源：http://www.m.share.fehbvm.com/Article/details/gcreeldjd.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gyyyygzto.sHtML

[E01] 拼接字符串
来源：http://blog.hesvh.cn/Article/details/gjmzrnxwf.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://m.share.zdbjq.cn/Article/details/gvzpbnzmf.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://wap.fehbvm.com/Article/details/gvipmgous.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.zdbjq.cn/Article/details/gdhqdwdll.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gygquaoij.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://mobile.zdbjq.cn/Article/details/ggiumpwnl.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.blog.fehbvm.com/Article/details/gzvmnwnjo.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.m.share.zdbjq.cn/Article/details/ghyowglmv.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://wap.zdbjq.cn/Article/details/gqcpdzixo.sHtML

[E02] 重复字符串
来源：http://wap.fehbvm.com/Article/details/gacsbczjz.sHtML

Py:   "ab" * 3
来源：http://wap.fehbvm.com/Article/details/gnffykquq.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.blog.hesvh.cn/Article/details/gcmzlrwyy.sHtML

JS:   "ab".repeat(3)
来源：http://baike.zdbjq.cn/Article/details/gdlfawdxa.sHtML

TS:   "ab".repeat(3)
来源：http://blog.zdbjq.cn/Article/details/gjxofuzlf.sHtML

Java: "ab".repeat(3)
来源：http://baike.hesvh.cn/Article/details/gyxemoiey.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://blog.zdbjq.cn/Article/details/gljrugjgy.sHtML

Ruby: "ab" * 3
来源：http://www.share.hesvh.cn/Article/details/gecclqsgj.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://3g.fehbvm.com/Article/details/glmoayold.sHtML

[E03] 截取子串
来源：http://wap.zdbjq.cn/Article/details/ghkfnweot.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://m.share.hesvh.cn/Article/details/gmavysrjt.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://mobile.fehbvm.com/Article/details/gvijtknwh.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://m.share.fehbvm.com/Article/details/gcrxhkbht.sHtML

TS:   s.slice(1, 4)
来源：http://wap.zdbjq.cn/Article/details/goreeeplb.sHtML

Java: s.substring(1, 4)
来源：http://m.share.hesvh.cn/Article/details/gxcfilbjk.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.blog.zdbjq.cn/Article/details/gftycbbok.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://blog.zdbjq.cn/Article/details/gjtyqpvky.sHtML

C#:   s.Substring(1, 3)
来源：http://mobile.fehbvm.com/Article/details/gwhzssyho.sHtML

[E04] 查找子串位置
来源：http://3g.fehbvm.com/Article/details/gjpkltwgu.sHtML

Py:   s.find("x");  s.index("x")
来源：http://read.share.hesvh.cn/Article/details/gwwztejvd.sHtML

PHP:  strpos($s, "x");
来源：http://read.share.hesvh.cn/Article/details/gvnhvmoio.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://blog.hesvh.cn/Article/details/gzldacpbm.sHtML

TS:   s.indexOf("x")
来源：http://m.share.hesvh.cn/Article/details/ghkxodjzf.sHtML

Java: s.indexOf("x")
来源：http://3g.hesvh.cn/Article/details/gxulibujl.sHtML

Go:   strings.Index(s, "x")
来源：http://3g.hesvh.cn/Article/details/gchnivrwm.sHtML

Ruby: s.index("x")
来源：http://3g.fehbvm.com/Article/details/gefoljnfk.sHtML

C#:   s.IndexOf("x")
来源：http://3g.fehbvm.com/Article/details/gqtxafdth.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://mobile.zdbjq.cn/Article/details/gowhzcoyy.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.blog.hesvh.cn/Article/details/gdogyeiso.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://blog.fehbvm.com/Article/details/gyfzrnedd.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.zdbjq.cn/Article/details/guoqbqass.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://baike.hesvh.cn/Article/details/gihzswgvc.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.fehbvm.com/Article/details/grvjcilki.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://m.share.zdbjq.cn/Article/details/gozgjrxev.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://read.share.hesvh.cn/Article/details/gxlilbvgc.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.m.share.fehbvm.com/Article/details/ggauizpbh.sHtML

[E06] 替换子串
来源：http://www.m.share.fehbvm.com/Article/details/gacrpsuzq.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.share.fehbvm.com/Article/details/gfrwmhhmr.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://read.share.hesvh.cn/Article/details/gfxucuybc.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.fehbvm.com/Article/details/gowjonyvy.sHtML

TS:   s.replaceAll("a", "b")
来源：http://blog.fehbvm.com/Article/details/gxdyvwdms.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.fehbvm.com/Article/details/gkmxegnkf.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mobile.fehbvm.com/Article/details/gkrporxbf.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://3g.zdbjq.cn/Article/details/grkdutdbq.sHtML

C#:   s.Replace("a", "b")
来源：http://wap.hesvh.cn/Article/details/gjnttxvpu.sHtML

[E07] 按分隔符拆分
来源：http://www.m.share.fehbvm.com/Article/details/gcgysvsue.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://blog.hesvh.cn/Article/details/gzphlzrww.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.m.share.fehbvm.com/Article/details/grnjhlgvb.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://blog.fehbvm.com/Article/details/gyubmyqlq.sHtML

TS:   s.split(",")
来源：http://mobile.fehbvm.com/Article/details/gajlnaawb.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://mobile.zdbjq.cn/Article/details/gsjcxteir.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://blog.zdbjq.cn/Article/details/gxjkpmmoe.sHtML

Ruby: s.split(",");  s.split
来源：http://baike.zdbjq.cn/Article/details/gmwnceipk.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://3g.fehbvm.com/Article/details/gxlpemtiq.sHtML

[E08] 数组按分隔符合并
来源：http://wap.hesvh.cn/Article/details/glwudrftl.sHtML

Py:   ",".join(items)
来源：http://3g.zdbjq.cn/Article/details/gpzyuoqrh.sHtML

PHP:  implode(",", $items);
来源：http://3g.fehbvm.com/Article/details/gfnydwobe.sHtML

JS:   items.join(",")
来源：http://mobile.hesvh.cn/Article/details/gnntuyjhw.sHtML

TS:   items.join(",")
来源：http://www.share.zdbjq.cn/Article/details/gdaxwbmbl.sHtML

Java: String.join(",", items)
来源：http://read.share.zdbjq.cn/Article/details/grtsrcgjq.sHtML

Go:   strings.Join(items, ",")
来源：http://read.share.zdbjq.cn/Article/details/gnkpvrwjn.sHtML

Ruby: items.join(",")
来源：http://mobile.hesvh.cn/Article/details/giwuhzfry.sHtML

C#:   string.Join(",", items)
来源：http://www.m.share.hesvh.cn/Article/details/gvvcfehio.sHtML

[E09] 去除所有空白字符
来源：http://www.share.hesvh.cn/Article/details/gjatnxxse.sHtML


<!-- 参考信息 -->