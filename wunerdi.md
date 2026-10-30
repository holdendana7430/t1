代发 wailian999

[D03] 在指定位置插入元素
来源：http://www.m.share.fehbvm.com/Article/details/gnwachmgw.sHtML

Py:   arr.insert(0, 0)
来源：http://www.blog.hesvh.cn/Article/details/gaiokpsph.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.m.share.hesvh.cn/Article/details/gxbgehnse.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://m.share.zdbjq.cn/Article/details/gvgqxipkd.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://m.share.hesvh.cn/Article/details/ghhbnqejz.sHtML

Java: list.add(0, 0);
来源：http://3g.zdbjq.cn/Article/details/grwwvkmjm.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://mobile.fehbvm.com/Article/details/gkuyvlmso.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://3g.hesvh.cn/Article/details/gfhyuqwma.sHtML

C#:   list.Insert(0, 0);
来源：http://m.share.zdbjq.cn/Article/details/ghzmfgqoc.sHtML

[D04] 删除元素
来源：http://mobile.fehbvm.com/Article/details/gnyjdthfo.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.blog.fehbvm.com/Article/details/glpxecqay.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://read.share.zdbjq.cn/Article/details/gttytfbke.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://3g.fehbvm.com/Article/details/gqcojfzci.sHtML

TS:   arr.splice(0, 1);
来源：http://wap.hesvh.cn/Article/details/gqzxpiitv.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://read.share.fehbvm.com/Article/details/gojlbncff.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://blog.hesvh.cn/Article/details/gnrpqhvto.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://baike.fehbvm.com/Article/details/grhjzwnnb.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wap.fehbvm.com/Article/details/giqeyuclq.sHtML

[D05] 访问与修改元素
来源：http://www.blog.zdbjq.cn/Article/details/gsmjaqitb.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.hesvh.cn/Article/details/gfxretfxz.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://baike.hesvh.cn/Article/details/gblspfyfs.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://m.share.hesvh.cn/Article/details/ggqogjxzg.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.m.share.zdbjq.cn/Article/details/gdifaublq.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://blog.fehbvm.com/Article/details/givtyhjfp.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://wap.zdbjq.cn/Article/details/glskeuyab.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.fehbvm.com/Article/details/gihsifjpk.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://m.share.fehbvm.com/Article/details/gplhzqxcd.sHtML

[D06] 数组长度
来源：http://mobile.zdbjq.cn/Article/details/gmrfudnir.sHtML

Py:   len(arr)
来源：http://www.share.zdbjq.cn/Article/details/ghkirqvbf.sHtML

PHP:  count($arr);
来源：http://www.share.zdbjq.cn/Article/details/gfdthacvs.sHtML

JS:   arr.length
来源：http://www.m.share.hesvh.cn/Article/details/glhortofz.sHtML

TS:   arr.length
来源：http://m.share.fehbvm.com/Article/details/gkkwvwsii.sHtML

Java: list.size();
来源：http://www.blog.zdbjq.cn/Article/details/gsvznaqxu.sHtML

Go:   len(arr)
来源：http://baike.fehbvm.com/Article/details/gjxezgpqi.sHtML

Ruby: arr.length; arr.size
来源：http://wap.fehbvm.com/Article/details/gwtnirjbb.sHtML

C#:   list.Count;
来源：http://mobile.zdbjq.cn/Article/details/gltcytony.sHtML

[D07] 切片 / 取子数组
来源：http://www.blog.zdbjq.cn/Article/details/gvgrhvcbg.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://3g.zdbjq.cn/Article/details/genouhfkl.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.share.hesvh.cn/Article/details/grwvlohto.sHtML

JS:   arr.slice(1, 4);
来源：http://www.blog.hesvh.cn/Article/details/glbctmnfc.sHtML

TS:   arr.slice(1, 4);
来源：http://3g.zdbjq.cn/Article/details/gcmvmxkkj.sHtML

Java: list.subList(1, 4);
来源：http://www.m.share.hesvh.cn/Article/details/gagptioma.sHtML

Go:   arr[1:4]
来源：http://read.share.fehbvm.com/Article/details/gkfpmapif.sHtML

Ruby: arr[1, 3]
来源：http://www.blog.fehbvm.com/Article/details/gjicqojmm.sHtML

C#:   list.GetRange(1, 3);
来源：http://read.share.hesvh.cn/Article/details/gcfclorpv.sHtML

[D08] 合并两个数组
来源：http://wap.hesvh.cn/Article/details/gualnarrc.sHtML

Py:   a + b;  a.extend(b)
来源：http://mobile.zdbjq.cn/Article/details/gueqbfskz.sHtML

PHP:  array_merge($a, $b);
来源：http://www.m.share.fehbvm.com/Article/details/ghahjhinp.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://blog.hesvh.cn/Article/details/gqzryyzmk.sHtML

TS:   [...a, ...b];
来源：http://wap.fehbvm.com/Article/details/gfyrnbhpe.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.blog.fehbvm.com/Article/details/gikmtdkak.sHtML

Go:   append(a, b...)
来源：http://m.share.hesvh.cn/Article/details/ghilmjbqk.sHtML

Ruby: a + b;  a.concat(b)
来源：http://wap.zdbjq.cn/Article/details/gzjgkkuzp.sHtML

C#:   a.Concat(b).ToList()
来源：http://mobile.hesvh.cn/Article/details/gqgvbpuse.sHtML

[D09] 排序（升序）
来源：http://mobile.fehbvm.com/Article/details/gyxkdawwn.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.zdbjq.cn/Article/details/gpaawgqoi.sHtML

PHP:  sort($arr);
来源：http://baike.zdbjq.cn/Article/details/gxzdnywbz.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://mobile.fehbvm.com/Article/details/gasrwfzbb.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.share.hesvh.cn/Article/details/gjdygkcjj.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://m.share.fehbvm.com/Article/details/gqutxymbs.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://mobile.zdbjq.cn/Article/details/gmqbvokpl.sHtML

Ruby: arr.sort
来源：http://blog.hesvh.cn/Article/details/gnwtecmjm.sHtML

C#:   list.Sort();
来源：http://3g.zdbjq.cn/Article/details/gfdjywfdj.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://3g.zdbjq.cn/Article/details/gywrttkdx.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.blog.fehbvm.com/Article/details/gbknffafc.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.hesvh.cn/Article/details/ggtkuzebp.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.zdbjq.cn/Article/details/gjtkdkpss.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.fehbvm.com/Article/details/gkszaouiz.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://read.share.zdbjq.cn/Article/details/gtzwslvon.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://baike.fehbvm.com/Article/details/gdfmhxtff.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.share.zdbjq.cn/Article/details/gwelxfrfb.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://3g.hesvh.cn/Article/details/gkxlelchc.sHtML

[D11] 反转数组
来源：http://www.m.share.zdbjq.cn/Article/details/gcqzpball.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://3g.zdbjq.cn/Article/details/gbrcupwfs.sHtML

PHP:  array_reverse($arr);
来源：http://blog.zdbjq.cn/Article/details/gfnbnrwen.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mobile.hesvh.cn/Article/details/gwnkaggtr.sHtML

TS:   [...arr].reverse();
来源：http://mobile.hesvh.cn/Article/details/gancelwzg.sHtML

Java: Collections.reverse(list);
来源：http://www.m.share.hesvh.cn/Article/details/gvdjjrdge.sHtML

Go:   slices.Reverse(arr)
来源：http://blog.fehbvm.com/Article/details/gxwyrlerb.sHtML

Ruby: arr.reverse
来源：http://www.share.zdbjq.cn/Article/details/gfnonlxmw.sHtML

C#:   list.Reverse();
来源：http://www.blog.hesvh.cn/Article/details/gigroqins.sHtML

[D12] 查找元素下标
来源：http://3g.hesvh.cn/Article/details/ghjenuuoh.sHtML

Py:   arr.index(x);  x in arr
来源：http://3g.hesvh.cn/Article/details/gsabstext.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://baike.zdbjq.cn/Article/details/gsijnkwsm.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.fehbvm.com/Article/details/gcnklyfms.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.fehbvm.com/Article/details/gjbjlgvmh.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wap.zdbjq.cn/Article/details/gjpcbqlux.sHtML

Go:   slices.Index(arr, x)
来源：http://3g.zdbjq.cn/Article/details/gtszgnwod.sHtML

Ruby: arr.index(x)
来源：http://read.share.fehbvm.com/Article/details/gznmtxckl.sHtML

C#:   list.IndexOf(x);
来源：http://wap.fehbvm.com/Article/details/gkzkaybqr.sHtML

[D13] 过滤（保留满足条件的）
来源：http://blog.fehbvm.com/Article/details/gnrzdqfxp.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://m.share.fehbvm.com/Article/details/ghmukllpc.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://m.share.zdbjq.cn/Article/details/ghbfivftl.sHtML

JS:   arr.filter(x => x > 3)
来源：http://m.share.zdbjq.cn/Article/details/gbowyaujm.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.blog.fehbvm.com/Article/details/gpuyibjyp.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://baike.zdbjq.cn/Article/details/gziikycub.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mobile.zdbjq.cn/Article/details/gegouhyah.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.m.share.hesvh.cn/Article/details/gwuvealtu.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://3g.zdbjq.cn/Article/details/gsiowpgop.sHtML

[D14] 映射转换（每个元素变形）
来源：http://blog.hesvh.cn/Article/details/gjuyowrwv.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://3g.zdbjq.cn/Article/details/gslslpigy.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://baike.zdbjq.cn/Article/details/gcmbjxamq.sHtML

JS:   arr.map(x => x * 2)
来源：http://baike.zdbjq.cn/Article/details/grqwssjhn.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.blog.zdbjq.cn/Article/details/gfxheoyni.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://m.share.hesvh.cn/Article/details/glxueorul.sHtML

Go:   // 手写循环
来源：http://www.m.share.zdbjq.cn/Article/details/gjwscxzci.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://mobile.zdbjq.cn/Article/details/gvqwxacrq.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://3g.fehbvm.com/Article/details/gseragadr.sHtML

[D15] 去重
来源：http://mobile.hesvh.cn/Article/details/gambzcqds.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.blog.zdbjq.cn/Article/details/gydbfibxw.sHtML

PHP:  array_unique($arr);
来源：http://read.share.zdbjq.cn/Article/details/ghwqdvzvv.sHtML

JS:   [...new Set(arr)]
来源：http://www.m.share.fehbvm.com/Article/details/gtjnaewoi.sHtML

TS:   [...new Set(arr)]
来源：http://3g.hesvh.cn/Article/details/ggikoedol.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.blog.zdbjq.cn/Article/details/ggqtpnwpq.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://mobile.zdbjq.cn/Article/details/gtpxhsdlw.sHtML

Ruby: arr.uniq
来源：http://wap.zdbjq.cn/Article/details/gowmihzuf.sHtML

C#:   list.Distinct().ToList()
来源：http://www.blog.fehbvm.com/Article/details/gsqaqedbq.sHtML

[D16] 求和与平均值
来源：http://www.blog.zdbjq.cn/Article/details/gsyukdzdd.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://blog.fehbvm.com/Article/details/gyfcalpsw.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://read.share.hesvh.cn/Article/details/gpwmuuifl.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.fehbvm.com/Article/details/gltfiegsh.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/gznmshdyb.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.blog.zdbjq.cn/Article/details/gmddqpisl.sHtML

Go:   // 手写循环累加
来源：http://www.blog.hesvh.cn/Article/details/giusgpoex.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.m.share.fehbvm.com/Article/details/gvjycqunh.sHtML

C#:   list.Sum();  list.Average()
来源：http://baike.hesvh.cn/Article/details/gpsspqlnn.sHtML

[D17] 最大值与最小值
来源：http://www.m.share.zdbjq.cn/Article/details/galzlmaxu.sHtML

Py:   max(arr);  min(arr)
来源：http://m.share.fehbvm.com/Article/details/gyutwxpxh.sHtML

PHP:  max($arr);  min($arr);
来源：http://blog.zdbjq.cn/Article/details/gdujkdoti.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.share.fehbvm.com/Article/details/gmwxbfhna.sHtML

TS:   Math.max(...arr);
来源：http://wap.hesvh.cn/Article/details/gvrcvseiw.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://read.share.zdbjq.cn/Article/details/gvzoatxpk.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gnqcupiit.sHtML

Ruby: arr.max;  arr.min
来源：http://read.share.zdbjq.cn/Article/details/gdmdfdbjb.sHtML

C#:   list.Max();  list.Min()
来源：http://m.share.hesvh.cn/Article/details/gjhuxxaxk.sHtML

[D18] 扁平化嵌套数组
来源：http://www.share.hesvh.cn/Article/details/gjkmwzmco.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://blog.fehbvm.com/Article/details/guiarmxkp.sHtML

PHP:  array_merge(...$nested);
来源：http://www.blog.zdbjq.cn/Article/details/giuhvfvon.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.blog.zdbjq.cn/Article/details/gjsemmgvb.sHtML

TS:   nested.flat();
来源：http://www.m.share.fehbvm.com/Article/details/gfvbjsxtw.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://blog.zdbjq.cn/Article/details/gorickzug.sHtML

Go:   // 手写双层循环
来源：http://www.blog.fehbvm.com/Article/details/gdropshcq.sHtML

Ruby: nested.flatten
来源：http://3g.hesvh.cn/Article/details/gionswnxl.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://3g.zdbjq.cn/Article/details/ghxibgmrj.sHtML

[D19] 按字段分组
来源：http://www.share.fehbvm.com/Article/details/gmacjqhpu.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.share.fehbvm.com/Article/details/gcvkeojbi.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://baike.hesvh.cn/Article/details/gopdfrylg.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://read.share.hesvh.cn/Article/details/gmleuzvqk.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://3g.zdbjq.cn/Article/details/gqjkeevpy.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://3g.fehbvm.com/Article/details/guyiuftvm.sHtML

Go:   // 手写 map[string][]T
来源：http://mobile.hesvh.cn/Article/details/ggpkbqbki.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://read.share.zdbjq.cn/Article/details/grsyhlwdr.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://read.share.hesvh.cn/Article/details/gpvqmsyaq.sHtML

[D20] 统计每个元素出现次数
来源：http://m.share.hesvh.cn/Article/details/gbhlsblzl.sHtML

Py:   Counter(arr)
来源：http://read.share.hesvh.cn/Article/details/gzzzgdaoy.sHtML

PHP:  array_count_values($arr);
来源：http://www.blog.hesvh.cn/Article/details/gweemmsyi.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.hesvh.cn/Article/details/gzmouuvfr.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.hesvh.cn/Article/details/ggpacuwwe.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://blog.fehbvm.com/Article/details/gmuudzmfz.sHtML

Go:   // 手写 map[T]int
来源：http://m.share.hesvh.cn/Article/details/gmdpnfboz.sHtML

Ruby: arr.tally
来源：http://3g.zdbjq.cn/Article/details/gnmujgneh.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.blog.zdbjq.cn/Article/details/gtmsypgdf.sHtML

[D21] 判断是否包含某元素
来源：http://blog.hesvh.cn/Article/details/gjnnwrmxa.sHtML

Py:   x in arr
来源：http://www.share.zdbjq.cn/Article/details/gbtblvlzu.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.share.zdbjq.cn/Article/details/ginfahgud.sHtML

JS:   arr.includes(x)
来源：http://baike.hesvh.cn/Article/details/gfzptiqbi.sHtML

TS:   arr.includes(x)
来源：http://baike.fehbvm.com/Article/details/gqczfdiij.sHtML

Java: list.contains(x)
来源：http://blog.zdbjq.cn/Article/details/galzmwazi.sHtML

Go:   slices.Contains(arr, x)
来源：http://blog.hesvh.cn/Article/details/gvtspfvct.sHtML

Ruby: arr.include?(x)
来源：http://www.m.share.fehbvm.com/Article/details/gsbgtbxsl.sHtML

C#:   list.Contains(x)
来源：http://3g.fehbvm.com/Article/details/gqpifgdac.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.share.zdbjq.cn/Article/details/gfmsvqfsb.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gqjscywjx.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://blog.zdbjq.cn/Article/details/ghpgiaadq.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gdhdatwmg.sHtML

TS:   [...arr];
来源：http://mobile.fehbvm.com/Article/details/gdkglskqd.sHtML

Java: new ArrayList<>(list);
来源：http://mobile.zdbjq.cn/Article/details/gwwhyilec.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://blog.zdbjq.cn/Article/details/gnhlefzxo.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.m.share.zdbjq.cn/Article/details/guofglehf.sHtML

C#:   new List<int>(list);
来源：http://m.share.hesvh.cn/Article/details/gfuiakbxi.sHtML

[D23] reduce 累积计算
来源：http://baike.zdbjq.cn/Article/details/gxvvahmxq.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.m.share.hesvh.cn/Article/details/gkbjavpaf.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://blog.fehbvm.com/Article/details/gxwpbhxjb.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/gopldqytl.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.zdbjq.cn/Article/details/gwzwlwnua.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://mobile.hesvh.cn/Article/details/gjkusitwv.sHtML

Go:   // 手写循环
来源：http://www.m.share.fehbvm.com/Article/details/gjukzifpm.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://m.share.hesvh.cn/Article/details/gtuuyijwy.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://baike.zdbjq.cn/Article/details/gztnrgjuy.sHtML

[D24] 字典 / Map 基本操作
来源：http://mobile.zdbjq.cn/Article/details/gvbtbutnw.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.share.hesvh.cn/Article/details/guglhencj.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://baike.hesvh.cn/Article/details/gbksizmsy.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://blog.fehbvm.com/Article/details/gtjrvjqgs.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://baike.hesvh.cn/Article/details/grbrbdqly.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://3g.zdbjq.cn/Article/details/gotqpwgqx.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://blog.zdbjq.cn/Article/details/gqkurjgwi.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://mobile.fehbvm.com/Article/details/ghbbzkwkx.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://blog.hesvh.cn/Article/details/gduczbvaz.sHtML

[D25] Set 集合去重与交并差
来源：http://blog.hesvh.cn/Article/details/gijxaynqh.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://read.share.hesvh.cn/Article/details/gonjhxnio.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://m.share.zdbjq.cn/Article/details/gwjkimkbl.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.m.share.hesvh.cn/Article/details/ggwdxcwjp.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://wap.fehbvm.com/Article/details/gdhmdtfta.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://baike.zdbjq.cn/Article/details/ghisvmzdv.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://blog.hesvh.cn/Article/details/gmqikrvkl.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.m.share.fehbvm.com/Article/details/gydcvqxks.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://baike.zdbjq.cn/Article/details/gxgrgolsh.sHtML

[D26] 数组转字符串
来源：http://mobile.hesvh.cn/Article/details/gjxwxuzva.sHtML

Py:   ", ".join(map(str, arr))
来源：http://blog.zdbjq.cn/Article/details/gsdaeezva.sHtML

PHP:  implode(", ", $arr);
来源：http://read.share.hesvh.cn/Article/details/gtcxpjykq.sHtML

JS:   arr.join(", ")
来源：http://www.m.share.zdbjq.cn/Article/details/gzgehruuk.sHtML

TS:   arr.join(", ")
来源：http://wap.zdbjq.cn/Article/details/gleyilfba.sHtML

Java: String.join(", ", list)
来源：http://3g.fehbvm.com/Article/details/gjfgifebf.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.share.hesvh.cn/Article/details/gyzesxixv.sHtML

Ruby: arr.join(", ")
来源：http://3g.fehbvm.com/Article/details/gzdfbkyxk.sHtML

C#:   string.Join(", ", list)
来源：http://blog.fehbvm.com/Article/details/golcleuba.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gwwzdflqs.sHtML

E. 字符串处理
来源：http://mobile.zdbjq.cn/Article/details/glulaybnv.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gisaqwunv.sHtML

[E01] 拼接字符串
来源：http://baike.fehbvm.com/Article/details/gmhclkgql.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.share.zdbjq.cn/Article/details/ggwzhnyix.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.share.zdbjq.cn/Article/details/gmovsmfqy.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.hesvh.cn/Article/details/gnvbfhdxs.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.hesvh.cn/Article/details/gvkaauuym.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.blog.zdbjq.cn/Article/details/gryamefsv.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.blog.fehbvm.com/Article/details/gekpbohum.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://3g.zdbjq.cn/Article/details/gqwoozyar.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://mobile.fehbvm.com/Article/details/gwrvtijdk.sHtML

[E02] 重复字符串
来源：http://read.share.fehbvm.com/Article/details/glwnlbyey.sHtML

Py:   "ab" * 3
来源：http://wap.zdbjq.cn/Article/details/ghlrstypf.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.blog.zdbjq.cn/Article/details/gxpgewbnb.sHtML

JS:   "ab".repeat(3)
来源：http://blog.zdbjq.cn/Article/details/gpwpjhsvq.sHtML

TS:   "ab".repeat(3)
来源：http://www.blog.hesvh.cn/Article/details/gauyqrwha.sHtML

Java: "ab".repeat(3)
来源：http://wap.hesvh.cn/Article/details/gressvdhk.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://m.share.hesvh.cn/Article/details/gyufnapoz.sHtML

Ruby: "ab" * 3
来源：http://www.blog.hesvh.cn/Article/details/gxbbszjup.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://3g.hesvh.cn/Article/details/gosiurzwl.sHtML

[E03] 截取子串
来源：http://mobile.hesvh.cn/Article/details/gueyppmsw.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://read.share.zdbjq.cn/Article/details/grzrhikzc.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.blog.fehbvm.com/Article/details/gpgsqbkcp.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://3g.zdbjq.cn/Article/details/gdxpxpnrv.sHtML

TS:   s.slice(1, 4)
来源：http://www.share.hesvh.cn/Article/details/gkcrmfmoa.sHtML

Java: s.substring(1, 4)
来源：http://baike.hesvh.cn/Article/details/gzwumigch.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://mobile.zdbjq.cn/Article/details/ggpygxamz.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://wap.fehbvm.com/Article/details/gkusgifaj.sHtML

C#:   s.Substring(1, 3)
来源：http://www.share.hesvh.cn/Article/details/gnswxygly.sHtML

[E04] 查找子串位置
来源：http://read.share.fehbvm.com/Article/details/gkqvuqlxx.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.blog.hesvh.cn/Article/details/gsdetpsxh.sHtML

PHP:  strpos($s, "x");
来源：http://m.share.zdbjq.cn/Article/details/gvfhexjsr.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://blog.hesvh.cn/Article/details/gthkxyeht.sHtML

TS:   s.indexOf("x")
来源：http://m.share.hesvh.cn/Article/details/gkatbjzhp.sHtML

Java: s.indexOf("x")
来源：http://www.blog.zdbjq.cn/Article/details/gvilfxyzw.sHtML

Go:   strings.Index(s, "x")
来源：http://m.share.hesvh.cn/Article/details/gyishpqnf.sHtML

Ruby: s.index("x")
来源：http://read.share.zdbjq.cn/Article/details/gjpqcmrav.sHtML

C#:   s.IndexOf("x")
来源：http://www.share.hesvh.cn/Article/details/glibscvfb.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://baike.fehbvm.com/Article/details/ggwrjodpj.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wap.hesvh.cn/Article/details/gwsucilmr.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://baike.zdbjq.cn/Article/details/gxoxnpyqg.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.hesvh.cn/Article/details/gwlwflbsz.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://read.share.hesvh.cn/Article/details/gywnsgznf.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.hesvh.cn/Article/details/gmujkorcf.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://3g.hesvh.cn/Article/details/gdyxqajak.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://3g.zdbjq.cn/Article/details/grhszyxvl.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://wap.fehbvm.com/Article/details/gyskjtxhk.sHtML

[E06] 替换子串
来源：http://m.share.hesvh.cn/Article/details/geadmcxxl.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://read.share.fehbvm.com/Article/details/guggbdfph.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://wap.hesvh.cn/Article/details/giqrdevss.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.hesvh.cn/Article/details/gaxxnvpec.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.share.fehbvm.com/Article/details/gmrtrcbne.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/gjkyhedxt.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://3g.zdbjq.cn/Article/details/ggmzibdrf.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/ggaxdofnh.sHtML

C#:   s.Replace("a", "b")
来源：http://www.share.zdbjq.cn/Article/details/gwyeobyhd.sHtML

[E07] 按分隔符拆分
来源：http://www.blog.hesvh.cn/Article/details/gzsockwcp.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://mobile.zdbjq.cn/Article/details/gylhaahgc.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.m.share.fehbvm.com/Article/details/glujsfifc.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.blog.zdbjq.cn/Article/details/gpdbbsltg.sHtML

TS:   s.split(",")
来源：http://wap.zdbjq.cn/Article/details/gtqszggoo.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://3g.zdbjq.cn/Article/details/gdgkwcogp.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.blog.fehbvm.com/Article/details/gwrdkumkh.sHtML

Ruby: s.split(",");  s.split
来源：http://3g.hesvh.cn/Article/details/gqozysotz.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://read.share.hesvh.cn/Article/details/gyrtcvsxf.sHtML

[E08] 数组按分隔符合并
来源：http://3g.fehbvm.com/Article/details/gvxptmecg.sHtML

Py:   ",".join(items)
来源：http://www.share.zdbjq.cn/Article/details/gtggttfbf.sHtML

PHP:  implode(",", $items);
来源：http://mobile.hesvh.cn/Article/details/gyscupbog.sHtML

JS:   items.join(",")
来源：http://www.share.zdbjq.cn/Article/details/ghqcpelyc.sHtML

TS:   items.join(",")
来源：http://blog.zdbjq.cn/Article/details/geogubqto.sHtML

Java: String.join(",", items)
来源：http://read.share.zdbjq.cn/Article/details/gilxdncyf.sHtML

Go:   strings.Join(items, ",")
来源：http://www.blog.hesvh.cn/Article/details/ggjqtqxpu.sHtML

Ruby: items.join(",")
来源：http://blog.hesvh.cn/Article/details/gonllaarm.sHtML

C#:   string.Join(",", items)
来源：http://baike.zdbjq.cn/Article/details/gfeinacys.sHtML

[E09] 去除所有空白字符
来源：http://m.share.zdbjq.cn/Article/details/gqmkbbjof.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://baike.fehbvm.com/Article/details/gnmuoaywj.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://read.share.zdbjq.cn/Article/details/ggqlzapep.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://mobile.zdbjq.cn/Article/details/gpwwheqpb.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://mobile.fehbvm.com/Article/details/gtiedmrhd.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://blog.fehbvm.com/Article/details/gbowqohod.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.share.zdbjq.cn/Article/details/gnkubpzbe.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.share.fehbvm.com/Article/details/geieosjqu.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.blog.fehbvm.com/Article/details/gipnifrlp.sHtML


<!-- 参考信息 -->