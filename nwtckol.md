代发 wailian999

TS:   arr.splice(0, 0, 0);
来源：http://wap.hesvh.cn/Article/details/gomntyyqy.sHtML

Java: list.add(0, 0);
来源：http://blog.hesvh.cn/Article/details/glqirznvl.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://wap.zdbjq.cn/Article/details/gqjvxebif.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://m.share.hesvh.cn/Article/details/ggvsevnoj.sHtML

C#:   list.Insert(0, 0);
来源：http://mobile.fehbvm.com/Article/details/gmhfedwif.sHtML

[D04] 删除元素
来源：http://wap.zdbjq.cn/Article/details/gbjasgcpk.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://blog.fehbvm.com/Article/details/gejovqbpi.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://3g.zdbjq.cn/Article/details/ghobsvgqp.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://read.share.zdbjq.cn/Article/details/guihtodoz.sHtML

TS:   arr.splice(0, 1);
来源：http://m.share.hesvh.cn/Article/details/gqptndkow.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.blog.fehbvm.com/Article/details/gghxgcwrk.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://3g.hesvh.cn/Article/details/gvxetdrfw.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.m.share.zdbjq.cn/Article/details/gltugeved.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.share.fehbvm.com/Article/details/gxxzrajsc.sHtML

[D05] 访问与修改元素
来源：http://wap.zdbjq.cn/Article/details/gcfqroyvz.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.zdbjq.cn/Article/details/grmhnjvzn.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://baike.fehbvm.com/Article/details/giwrxeeta.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://3g.hesvh.cn/Article/details/gfzmhxedn.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.blog.hesvh.cn/Article/details/gkawnpvss.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.share.hesvh.cn/Article/details/gyphertcq.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://wap.zdbjq.cn/Article/details/giwcawdeg.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.zdbjq.cn/Article/details/gxybsflhm.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://3g.fehbvm.com/Article/details/grhursmpj.sHtML

[D06] 数组长度
来源：http://www.m.share.zdbjq.cn/Article/details/gaezdpqty.sHtML

Py:   len(arr)
来源：http://mobile.hesvh.cn/Article/details/gfvvfpzoo.sHtML

PHP:  count($arr);
来源：http://read.share.hesvh.cn/Article/details/gnfjwukdz.sHtML

JS:   arr.length
来源：http://wap.zdbjq.cn/Article/details/giwrowewh.sHtML

TS:   arr.length
来源：http://blog.fehbvm.com/Article/details/gqxdnctis.sHtML

Java: list.size();
来源：http://www.m.share.zdbjq.cn/Article/details/gikcqpykl.sHtML

Go:   len(arr)
来源：http://3g.fehbvm.com/Article/details/gmmmbmtev.sHtML

Ruby: arr.length; arr.size
来源：http://mobile.fehbvm.com/Article/details/ggwvpuhwp.sHtML

C#:   list.Count;
来源：http://m.share.hesvh.cn/Article/details/ghittazja.sHtML

[D07] 切片 / 取子数组
来源：http://www.blog.zdbjq.cn/Article/details/gdfamlopl.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://blog.zdbjq.cn/Article/details/gvqtdesdh.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.share.zdbjq.cn/Article/details/gpsglgpbi.sHtML

JS:   arr.slice(1, 4);
来源：http://read.share.hesvh.cn/Article/details/gouuheitq.sHtML

TS:   arr.slice(1, 4);
来源：http://www.share.hesvh.cn/Article/details/gyeygcylw.sHtML

Java: list.subList(1, 4);
来源：http://www.m.share.fehbvm.com/Article/details/goikoodly.sHtML

Go:   arr[1:4]
来源：http://baike.zdbjq.cn/Article/details/grxhrscct.sHtML

Ruby: arr[1, 3]
来源：http://baike.hesvh.cn/Article/details/gskdqzbri.sHtML

C#:   list.GetRange(1, 3);
来源：http://mobile.zdbjq.cn/Article/details/gpnhovtmo.sHtML

[D08] 合并两个数组
来源：http://www.share.zdbjq.cn/Article/details/gdfgsylrh.sHtML

Py:   a + b;  a.extend(b)
来源：http://mobile.fehbvm.com/Article/details/gilqnwxph.sHtML

PHP:  array_merge($a, $b);
来源：http://read.share.zdbjq.cn/Article/details/gjihkdgat.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://read.share.hesvh.cn/Article/details/glmwrsoqw.sHtML

TS:   [...a, ...b];
来源：http://wap.hesvh.cn/Article/details/gacbybzsq.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://baike.zdbjq.cn/Article/details/guappzfek.sHtML

Go:   append(a, b...)
来源：http://blog.fehbvm.com/Article/details/gppudiyra.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.blog.zdbjq.cn/Article/details/gxxfdqlhd.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.blog.fehbvm.com/Article/details/gdedhdlhe.sHtML

[D09] 排序（升序）
来源：http://www.m.share.fehbvm.com/Article/details/gearksydc.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.fehbvm.com/Article/details/gwskipbvz.sHtML

PHP:  sort($arr);
来源：http://wap.hesvh.cn/Article/details/gmcdvazou.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.share.hesvh.cn/Article/details/glbaopoxn.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://read.share.hesvh.cn/Article/details/gfikuiwaj.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://blog.hesvh.cn/Article/details/gjggkzebo.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://3g.hesvh.cn/Article/details/giqcsmlsx.sHtML

Ruby: arr.sort
来源：http://mobile.zdbjq.cn/Article/details/gtggndjxt.sHtML

C#:   list.Sort();
来源：http://mobile.zdbjq.cn/Article/details/gsfnhfpkl.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://m.share.fehbvm.com/Article/details/gapecvdgy.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.share.hesvh.cn/Article/details/gacsldgms.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.fehbvm.com/Article/details/gnkhonkwl.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.fehbvm.com/Article/details/gilzfkykc.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.zdbjq.cn/Article/details/glmjgkhjj.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://3g.fehbvm.com/Article/details/gjuexzsrh.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://3g.fehbvm.com/Article/details/gjakbphna.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.share.hesvh.cn/Article/details/gmdghtdpr.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.share.fehbvm.com/Article/details/ghqcbmddy.sHtML

[D11] 反转数组
来源：http://mobile.hesvh.cn/Article/details/gpbsblhwq.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://wap.hesvh.cn/Article/details/guplwrzao.sHtML

PHP:  array_reverse($arr);
来源：http://3g.zdbjq.cn/Article/details/giyetgsjx.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://baike.hesvh.cn/Article/details/gpkggdlfb.sHtML

TS:   [...arr].reverse();
来源：http://blog.fehbvm.com/Article/details/gscxnuyfg.sHtML

Java: Collections.reverse(list);
来源：http://m.share.hesvh.cn/Article/details/gvoajeahd.sHtML

Go:   slices.Reverse(arr)
来源：http://baike.zdbjq.cn/Article/details/ggtstvjha.sHtML

Ruby: arr.reverse
来源：http://mobile.zdbjq.cn/Article/details/gdczlfhde.sHtML

C#:   list.Reverse();
来源：http://mobile.zdbjq.cn/Article/details/gznyftxjq.sHtML

[D12] 查找元素下标
来源：http://mobile.zdbjq.cn/Article/details/gssxnqjva.sHtML

Py:   arr.index(x);  x in arr
来源：http://mobile.fehbvm.com/Article/details/gvkdsfcig.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://3g.fehbvm.com/Article/details/gxsyzlwth.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.fehbvm.com/Article/details/gyakrddai.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.fehbvm.com/Article/details/gwjvbpagi.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wap.zdbjq.cn/Article/details/gpqsdegxn.sHtML

Go:   slices.Index(arr, x)
来源：http://wap.zdbjq.cn/Article/details/gjgiqpdbw.sHtML

Ruby: arr.index(x)
来源：http://mobile.fehbvm.com/Article/details/gjwgjcnjm.sHtML

C#:   list.IndexOf(x);
来源：http://wap.hesvh.cn/Article/details/gvclnefoz.sHtML

[D13] 过滤（保留满足条件的）
来源：http://read.share.fehbvm.com/Article/details/gdwijtwgq.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://m.share.zdbjq.cn/Article/details/gzryxmqfe.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.blog.zdbjq.cn/Article/details/gsejpnpbh.sHtML

JS:   arr.filter(x => x > 3)
来源：http://m.share.zdbjq.cn/Article/details/gmazfrcri.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.m.share.hesvh.cn/Article/details/gcqdqefeo.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://read.share.fehbvm.com/Article/details/gqynxefkl.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://3g.fehbvm.com/Article/details/godrxpnfn.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://blog.hesvh.cn/Article/details/gvupizdby.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://m.share.fehbvm.com/Article/details/gakcjspal.sHtML

[D14] 映射转换（每个元素变形）
来源：http://baike.fehbvm.com/Article/details/gpvgkeffw.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.blog.zdbjq.cn/Article/details/gapsbpnfj.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mobile.hesvh.cn/Article/details/gbrwsbdkh.sHtML

JS:   arr.map(x => x * 2)
来源：http://read.share.hesvh.cn/Article/details/gmcyodewt.sHtML

TS:   arr.map(x => x * 2)
来源：http://read.share.hesvh.cn/Article/details/gnkwmclhg.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://blog.zdbjq.cn/Article/details/ggqmhhibc.sHtML

Go:   // 手写循环
来源：http://read.share.fehbvm.com/Article/details/guodhrtis.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.blog.hesvh.cn/Article/details/goneaemcr.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.share.hesvh.cn/Article/details/gvmikines.sHtML

[D15] 去重
来源：http://www.m.share.fehbvm.com/Article/details/gshvtknbh.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.share.hesvh.cn/Article/details/gvupvopuh.sHtML

PHP:  array_unique($arr);
来源：http://baike.zdbjq.cn/Article/details/gclbotqua.sHtML

JS:   [...new Set(arr)]
来源：http://www.blog.fehbvm.com/Article/details/gwdtauaqq.sHtML

TS:   [...new Set(arr)]
来源：http://wap.fehbvm.com/Article/details/gusbeweqc.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.share.zdbjq.cn/Article/details/gpcnltzam.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://blog.hesvh.cn/Article/details/glrnotvdd.sHtML

Ruby: arr.uniq
来源：http://m.share.fehbvm.com/Article/details/gmsewmxhp.sHtML

C#:   list.Distinct().ToList()
来源：http://read.share.zdbjq.cn/Article/details/gylzvgmle.sHtML

[D16] 求和与平均值
来源：http://wap.fehbvm.com/Article/details/gcwieaooh.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wap.zdbjq.cn/Article/details/gtcrpppgb.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wap.zdbjq.cn/Article/details/gsobrqyyp.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.fehbvm.com/Article/details/glxmsttiw.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.hesvh.cn/Article/details/gakvhucgg.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://read.share.zdbjq.cn/Article/details/gntqmltfy.sHtML

Go:   // 手写循环累加
来源：http://m.share.hesvh.cn/Article/details/glpbfidev.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mobile.zdbjq.cn/Article/details/gsykyqhpp.sHtML

C#:   list.Sum();  list.Average()
来源：http://mobile.fehbvm.com/Article/details/gtrhmbbde.sHtML

[D17] 最大值与最小值
来源：http://3g.fehbvm.com/Article/details/gogbagivz.sHtML

Py:   max(arr);  min(arr)
来源：http://blog.zdbjq.cn/Article/details/gzxngveuf.sHtML

PHP:  max($arr);  min($arr);
来源：http://read.share.fehbvm.com/Article/details/glsgbwfsm.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://read.share.hesvh.cn/Article/details/gbpaazlsw.sHtML

TS:   Math.max(...arr);
来源：http://blog.hesvh.cn/Article/details/gmnmftrrh.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.blog.hesvh.cn/Article/details/gfmllfntw.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.blog.fehbvm.com/Article/details/gtnjgcphh.sHtML

Ruby: arr.max;  arr.min
来源：http://baike.fehbvm.com/Article/details/gmkwhlqar.sHtML

C#:   list.Max();  list.Min()
来源：http://baike.hesvh.cn/Article/details/ghjheujbo.sHtML

[D18] 扁平化嵌套数组
来源：http://www.share.fehbvm.com/Article/details/gxxycigbl.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://3g.hesvh.cn/Article/details/gbvascagi.sHtML

PHP:  array_merge(...$nested);
来源：http://www.m.share.hesvh.cn/Article/details/gyzwnokys.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://baike.fehbvm.com/Article/details/gdjdgfdqz.sHtML

TS:   nested.flat();
来源：http://blog.zdbjq.cn/Article/details/gcnizfbye.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://baike.fehbvm.com/Article/details/gxilxbhub.sHtML

Go:   // 手写双层循环
来源：http://www.blog.hesvh.cn/Article/details/gwcfirjfa.sHtML

Ruby: nested.flatten
来源：http://baike.zdbjq.cn/Article/details/gfwystxxs.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://mobile.zdbjq.cn/Article/details/gydwkblxj.sHtML

[D19] 按字段分组
来源：http://read.share.fehbvm.com/Article/details/gdpooiygb.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.blog.fehbvm.com/Article/details/gtafvfnot.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mobile.hesvh.cn/Article/details/gfrttvvkr.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://read.share.fehbvm.com/Article/details/glhdiiudq.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://baike.fehbvm.com/Article/details/guanztiyu.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://read.share.hesvh.cn/Article/details/gvprnwyfa.sHtML

Go:   // 手写 map[string][]T
来源：http://3g.hesvh.cn/Article/details/glyhlyekt.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://blog.hesvh.cn/Article/details/gucfekiyw.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://3g.zdbjq.cn/Article/details/gfunzdomi.sHtML

[D20] 统计每个元素出现次数
来源：http://mobile.hesvh.cn/Article/details/gkqmjbrga.sHtML

Py:   Counter(arr)
来源：http://mobile.hesvh.cn/Article/details/gdtbkzyae.sHtML

PHP:  array_count_values($arr);
来源：http://wap.fehbvm.com/Article/details/gffaoeneh.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.hesvh.cn/Article/details/gbnzrfvid.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.fehbvm.com/Article/details/gifxuwdwm.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://read.share.hesvh.cn/Article/details/grwhptdem.sHtML

Go:   // 手写 map[T]int
来源：http://www.m.share.fehbvm.com/Article/details/gwxbuhmsh.sHtML

Ruby: arr.tally
来源：http://read.share.fehbvm.com/Article/details/gvgpnlefb.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://baike.zdbjq.cn/Article/details/gcadolwtn.sHtML

[D21] 判断是否包含某元素
来源：http://mobile.zdbjq.cn/Article/details/gciydmtmu.sHtML

Py:   x in arr
来源：http://www.share.fehbvm.com/Article/details/gswldplie.sHtML

PHP:  in_array($x, $arr, true);
来源：http://baike.fehbvm.com/Article/details/gyxqaghbg.sHtML

JS:   arr.includes(x)
来源：http://www.m.share.fehbvm.com/Article/details/gkjauhiun.sHtML

TS:   arr.includes(x)
来源：http://m.share.hesvh.cn/Article/details/gxpvhkvom.sHtML

Java: list.contains(x)
来源：http://3g.zdbjq.cn/Article/details/giydjhrcw.sHtML

Go:   slices.Contains(arr, x)
来源：http://mobile.hesvh.cn/Article/details/glqmemyfc.sHtML

Ruby: arr.include?(x)
来源：http://www.m.share.hesvh.cn/Article/details/gfsixaoal.sHtML

C#:   list.Contains(x)
来源：http://wap.zdbjq.cn/Article/details/gxemgmxzi.sHtML

[D22] 复制数组（避免共享引用）
来源：http://read.share.zdbjq.cn/Article/details/gwtikvwsp.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.share.zdbjq.cn/Article/details/gyqtxiojx.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://mobile.zdbjq.cn/Article/details/gvfjsyfec.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://read.share.hesvh.cn/Article/details/gcwmzhkrk.sHtML

TS:   [...arr];
来源：http://www.blog.zdbjq.cn/Article/details/gffmrgvgf.sHtML

Java: new ArrayList<>(list);
来源：http://www.blog.hesvh.cn/Article/details/gkqtnegay.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://blog.hesvh.cn/Article/details/gxymgugxl.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.m.share.zdbjq.cn/Article/details/gjrqiqmgk.sHtML

C#:   new List<int>(list);
来源：http://3g.fehbvm.com/Article/details/gvigawtaf.sHtML

[D23] reduce 累积计算
来源：http://blog.fehbvm.com/Article/details/gkwkjzefs.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/guynyrrdj.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.blog.zdbjq.cn/Article/details/gzyrlsftq.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.fehbvm.com/Article/details/guxmkuwtk.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.fehbvm.com/Article/details/goabkihfj.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://wap.zdbjq.cn/Article/details/gycfovqwo.sHtML

Go:   // 手写循环
来源：http://www.m.share.fehbvm.com/Article/details/gnwtajuyl.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.m.share.zdbjq.cn/Article/details/gbmxkpztc.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mobile.fehbvm.com/Article/details/giebpifug.sHtML

[D24] 字典 / Map 基本操作
来源：http://m.share.hesvh.cn/Article/details/gignbdjjn.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.blog.zdbjq.cn/Article/details/gdrjjachi.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://baike.hesvh.cn/Article/details/ggunkvxfg.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.share.zdbjq.cn/Article/details/gvlmvitfp.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.share.hesvh.cn/Article/details/gjgbxpwza.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://m.share.zdbjq.cn/Article/details/gkfabxdnd.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://m.share.fehbvm.com/Article/details/gagqlihdp.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://blog.zdbjq.cn/Article/details/gvtapfhlv.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://baike.hesvh.cn/Article/details/gxjnjglhe.sHtML

[D25] Set 集合去重与交并差
来源：http://wap.fehbvm.com/Article/details/gjasxacvt.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://baike.fehbvm.com/Article/details/gepzskqmd.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://3g.hesvh.cn/Article/details/gnjojvpsg.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://read.share.zdbjq.cn/Article/details/ggdadrmax.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.share.zdbjq.cn/Article/details/gezlmstml.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://mobile.zdbjq.cn/Article/details/gjzdsvcvr.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.blog.zdbjq.cn/Article/details/gzjdpnqsp.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.m.share.zdbjq.cn/Article/details/grocjwccr.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mobile.fehbvm.com/Article/details/gfvzjbivy.sHtML

[D26] 数组转字符串
来源：http://blog.zdbjq.cn/Article/details/ghqyiibcc.sHtML

Py:   ", ".join(map(str, arr))
来源：http://m.share.zdbjq.cn/Article/details/gibzuhofb.sHtML

PHP:  implode(", ", $arr);
来源：http://3g.fehbvm.com/Article/details/gltsrwbiy.sHtML

JS:   arr.join(", ")
来源：http://blog.hesvh.cn/Article/details/gugjoljgu.sHtML

TS:   arr.join(", ")
来源：http://www.m.share.fehbvm.com/Article/details/gimneykjt.sHtML

Java: String.join(", ", list)
来源：http://m.share.hesvh.cn/Article/details/gthukxbpx.sHtML

Go:   strings.Join(strs, ", ")
来源：http://baike.fehbvm.com/Article/details/ghtjatiec.sHtML

Ruby: arr.join(", ")
来源：http://www.share.fehbvm.com/Article/details/gavgpmxck.sHtML

C#:   string.Join(", ", list)
来源：http://read.share.fehbvm.com/Article/details/gqjxdyxfh.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gqofalhhm.sHtML

E. 字符串处理
来源：http://www.blog.hesvh.cn/Article/details/glvuqhkrx.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/guacyzpwp.sHtML

[E01] 拼接字符串
来源：http://m.share.fehbvm.com/Article/details/gnaugmfxo.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://blog.fehbvm.com/Article/details/gwnnebizt.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://baike.zdbjq.cn/Article/details/gkwiwlfka.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.hesvh.cn/Article/details/ggcwzqkyw.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.zdbjq.cn/Article/details/gdjjgrbga.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://wap.hesvh.cn/Article/details/gefbpumnx.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://3g.hesvh.cn/Article/details/gsfhhnzou.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wap.fehbvm.com/Article/details/gitmocdgg.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://blog.zdbjq.cn/Article/details/gedeyfxxo.sHtML

[E02] 重复字符串
来源：http://baike.hesvh.cn/Article/details/gjfviemiw.sHtML

Py:   "ab" * 3
来源：http://mobile.fehbvm.com/Article/details/ghinyencu.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.blog.hesvh.cn/Article/details/gdjumpchi.sHtML

JS:   "ab".repeat(3)
来源：http://read.share.zdbjq.cn/Article/details/grdhtzbuh.sHtML

TS:   "ab".repeat(3)
来源：http://www.share.zdbjq.cn/Article/details/gcwswunom.sHtML

Java: "ab".repeat(3)
来源：http://www.share.fehbvm.com/Article/details/grnrlctjo.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.blog.hesvh.cn/Article/details/gctfeybsa.sHtML

Ruby: "ab" * 3
来源：http://www.blog.hesvh.cn/Article/details/gtvvoxsuo.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://mobile.fehbvm.com/Article/details/gmjomigqk.sHtML

[E03] 截取子串
来源：http://3g.fehbvm.com/Article/details/gnvllxtst.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wap.zdbjq.cn/Article/details/gvzovbmwi.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://3g.fehbvm.com/Article/details/gjnljcdfj.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.m.share.zdbjq.cn/Article/details/gskqnyjln.sHtML

TS:   s.slice(1, 4)
来源：http://m.share.fehbvm.com/Article/details/grmnuwegb.sHtML

Java: s.substring(1, 4)
来源：http://www.share.zdbjq.cn/Article/details/gufcgbaot.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://read.share.hesvh.cn/Article/details/gpmlllqou.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://wap.hesvh.cn/Article/details/gukejmzdk.sHtML

C#:   s.Substring(1, 3)
来源：http://read.share.hesvh.cn/Article/details/galijvwou.sHtML

[E04] 查找子串位置
来源：http://www.blog.fehbvm.com/Article/details/gxhgsbpka.sHtML

Py:   s.find("x");  s.index("x")
来源：http://baike.fehbvm.com/Article/details/gnzahhdee.sHtML

PHP:  strpos($s, "x");
来源：http://3g.fehbvm.com/Article/details/gemrtamgx.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://mobile.hesvh.cn/Article/details/gyvssspfb.sHtML

TS:   s.indexOf("x")
来源：http://blog.hesvh.cn/Article/details/gcivwrimg.sHtML

Java: s.indexOf("x")
来源：http://read.share.fehbvm.com/Article/details/gsttqeoqi.sHtML

Go:   strings.Index(s, "x")
来源：http://read.share.hesvh.cn/Article/details/gnnhjzriw.sHtML

Ruby: s.index("x")
来源：http://wap.zdbjq.cn/Article/details/gjxufvuar.sHtML

C#:   s.IndexOf("x")
来源：http://blog.zdbjq.cn/Article/details/gqgzvufij.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://mobile.hesvh.cn/Article/details/grxdymibg.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://read.share.fehbvm.com/Article/details/gxepparbc.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wap.hesvh.cn/Article/details/gbzuehnls.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.hesvh.cn/Article/details/gxcylgtrn.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://mobile.hesvh.cn/Article/details/gryrsxauc.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.hesvh.cn/Article/details/grlyywmwo.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wap.hesvh.cn/Article/details/gjujguwwn.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.m.share.hesvh.cn/Article/details/glqbxjiio.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://blog.hesvh.cn/Article/details/gsypnqsjv.sHtML

[E06] 替换子串
来源：http://blog.zdbjq.cn/Article/details/glajiaaeu.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.share.zdbjq.cn/Article/details/gifomjame.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://3g.fehbvm.com/Article/details/gemayosqj.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.fehbvm.com/Article/details/gydwgnlbo.sHtML

TS:   s.replaceAll("a", "b")
来源：http://baike.zdbjq.cn/Article/details/giwhheamp.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.hesvh.cn/Article/details/gfwhjapxj.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.share.hesvh.cn/Article/details/gpjqwlsrc.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://3g.zdbjq.cn/Article/details/gwmlxtihv.sHtML

C#:   s.Replace("a", "b")
来源：http://www.blog.hesvh.cn/Article/details/gkbvhvabd.sHtML

[E07] 按分隔符拆分
来源：http://www.m.share.hesvh.cn/Article/details/gvlifzvpi.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://mobile.hesvh.cn/Article/details/gygytsgba.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://baike.fehbvm.com/Article/details/gssuwcdvq.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://wap.zdbjq.cn/Article/details/ghtqlskdf.sHtML

TS:   s.split(",")
来源：http://www.share.fehbvm.com/Article/details/giydjimpl.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://blog.fehbvm.com/Article/details/ggclirjcz.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wap.fehbvm.com/Article/details/gohxeqjvh.sHtML

Ruby: s.split(",");  s.split
来源：http://www.blog.hesvh.cn/Article/details/glwexeatw.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://baike.fehbvm.com/Article/details/gehaaylzi.sHtML

[E08] 数组按分隔符合并
来源：http://mobile.hesvh.cn/Article/details/gaazrwvwn.sHtML

Py:   ",".join(items)
来源：http://read.share.hesvh.cn/Article/details/gtakfhumn.sHtML

PHP:  implode(",", $items);
来源：http://mobile.zdbjq.cn/Article/details/gicjmaesb.sHtML

JS:   items.join(",")
来源：http://m.share.fehbvm.com/Article/details/gpukpwlpg.sHtML

TS:   items.join(",")
来源：http://wap.zdbjq.cn/Article/details/gyouvcrkb.sHtML

Java: String.join(",", items)
来源：http://read.share.zdbjq.cn/Article/details/gjmuqkbmw.sHtML

Go:   strings.Join(items, ",")
来源：http://blog.hesvh.cn/Article/details/gdwjxrwgb.sHtML

Ruby: items.join(",")
来源：http://www.blog.zdbjq.cn/Article/details/gxbvdoxcs.sHtML

C#:   string.Join(",", items)
来源：http://baike.fehbvm.com/Article/details/gurlggvaf.sHtML

[E09] 去除所有空白字符
来源：http://read.share.hesvh.cn/Article/details/gxlnbgiei.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.share.zdbjq.cn/Article/details/gavblrruz.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://mobile.hesvh.cn/Article/details/gkupsmgyg.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.blog.fehbvm.com/Article/details/grumpbvei.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://3g.hesvh.cn/Article/details/gqbqekpku.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://3g.zdbjq.cn/Article/details/gomkkejpv.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://read.share.fehbvm.com/Article/details/gonvpksta.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.blog.fehbvm.com/Article/details/glzhnsory.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.m.share.fehbvm.com/Article/details/ghupzyrwr.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.m.share.hesvh.cn/Article/details/gbtdncgcu.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.share.zdbjq.cn/Article/details/gsdyeagym.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://read.share.fehbvm.com/Article/details/gczrjnsom.sHtML

JS:   "7".padStart(3, "0")
来源：http://baike.fehbvm.com/Article/details/ghpsvankl.sHtML


<!-- 参考信息 -->