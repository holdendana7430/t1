代发 wailian999

C#:   list.Insert(0, 0);
来源：http://read.share.hesvh.cn/Article/details/gltbstszt.sHtML

[D04] 删除元素
来源：http://mobile.fehbvm.com/Article/details/ghxlboidq.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://3g.zdbjq.cn/Article/details/gadnvybnh.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.m.share.fehbvm.com/Article/details/gfyowimrx.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mobile.zdbjq.cn/Article/details/ggdazksih.sHtML

TS:   arr.splice(0, 1);
来源：http://mobile.zdbjq.cn/Article/details/grsuhbvvj.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gyanjmfyc.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://m.share.hesvh.cn/Article/details/gloajgulr.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://m.share.hesvh.cn/Article/details/glquljnms.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://mobile.zdbjq.cn/Article/details/grqzeuzie.sHtML

[D05] 访问与修改元素
来源：http://www.m.share.fehbvm.com/Article/details/gbzwnoimt.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.zdbjq.cn/Article/details/goxemibne.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.m.share.zdbjq.cn/Article/details/gtudkucvt.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://read.share.hesvh.cn/Article/details/glxnwfyyo.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://mobile.fehbvm.com/Article/details/gccoodiqf.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://blog.hesvh.cn/Article/details/grgutibff.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://m.share.fehbvm.com/Article/details/gghadglyz.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.hesvh.cn/Article/details/gvurnlbtj.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://wap.hesvh.cn/Article/details/gybudbipd.sHtML

[D06] 数组长度
来源：http://wap.zdbjq.cn/Article/details/ghwejcscb.sHtML

Py:   len(arr)
来源：http://wap.hesvh.cn/Article/details/gxvoxmhvf.sHtML

PHP:  count($arr);
来源：http://baike.zdbjq.cn/Article/details/gwaqpyiqw.sHtML

JS:   arr.length
来源：http://www.m.share.fehbvm.com/Article/details/gsypvrxmk.sHtML

TS:   arr.length
来源：http://read.share.zdbjq.cn/Article/details/gpprsvfym.sHtML

Java: list.size();
来源：http://wap.zdbjq.cn/Article/details/gvyatztpi.sHtML

Go:   len(arr)
来源：http://read.share.zdbjq.cn/Article/details/gbilgpavj.sHtML

Ruby: arr.length; arr.size
来源：http://wap.hesvh.cn/Article/details/ggbsawlna.sHtML

C#:   list.Count;
来源：http://read.share.hesvh.cn/Article/details/gfdjrywsf.sHtML

[D07] 切片 / 取子数组
来源：http://wap.zdbjq.cn/Article/details/gzwtoncjm.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://baike.zdbjq.cn/Article/details/gtxwnfpbs.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.m.share.fehbvm.com/Article/details/grncvbywm.sHtML

JS:   arr.slice(1, 4);
来源：http://www.blog.hesvh.cn/Article/details/gjskdczmf.sHtML

TS:   arr.slice(1, 4);
来源：http://m.share.fehbvm.com/Article/details/gkpjxqykg.sHtML

Java: list.subList(1, 4);
来源：http://www.share.zdbjq.cn/Article/details/goweduyai.sHtML

Go:   arr[1:4]
来源：http://read.share.hesvh.cn/Article/details/gjpyfkhvz.sHtML

Ruby: arr[1, 3]
来源：http://www.share.fehbvm.com/Article/details/gyhugmogw.sHtML

C#:   list.GetRange(1, 3);
来源：http://read.share.zdbjq.cn/Article/details/ggcwjldoh.sHtML

[D08] 合并两个数组
来源：http://read.share.zdbjq.cn/Article/details/gdustgjoa.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.blog.zdbjq.cn/Article/details/gcybzcxtc.sHtML

PHP:  array_merge($a, $b);
来源：http://baike.hesvh.cn/Article/details/ggnqhkvcl.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://mobile.zdbjq.cn/Article/details/gjehvgajc.sHtML

TS:   [...a, ...b];
来源：http://www.m.share.fehbvm.com/Article/details/glxvueyit.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://read.share.zdbjq.cn/Article/details/gfblbnbzj.sHtML

Go:   append(a, b...)
来源：http://www.m.share.hesvh.cn/Article/details/ggceouttl.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.share.zdbjq.cn/Article/details/gqbbqjxhd.sHtML

C#:   a.Concat(b).ToList()
来源：http://mobile.fehbvm.com/Article/details/gkyhnscms.sHtML

[D09] 排序（升序）
来源：http://www.m.share.zdbjq.cn/Article/details/gjzrhcjuh.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.fehbvm.com/Article/details/gyoroldvx.sHtML

PHP:  sort($arr);
来源：http://m.share.zdbjq.cn/Article/details/gfqhalrec.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://read.share.zdbjq.cn/Article/details/glltwzqms.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://wap.hesvh.cn/Article/details/gztriflgs.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.blog.fehbvm.com/Article/details/ggrnchnfc.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gojudylkq.sHtML

Ruby: arr.sort
来源：http://blog.hesvh.cn/Article/details/ggamepdkv.sHtML

C#:   list.Sort();
来源：http://m.share.hesvh.cn/Article/details/glcygflqi.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://wap.zdbjq.cn/Article/details/gznaivgqr.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://blog.fehbvm.com/Article/details/gadasuvxy.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.zdbjq.cn/Article/details/giopiladd.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.fehbvm.com/Article/details/ggydbvock.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.fehbvm.com/Article/details/gzfwcjqau.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://mobile.hesvh.cn/Article/details/gqcrpoozp.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://baike.hesvh.cn/Article/details/gwqfqakan.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://m.share.fehbvm.com/Article/details/gmjvgkfqy.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://blog.hesvh.cn/Article/details/gcldbauol.sHtML

[D11] 反转数组
来源：http://wap.fehbvm.com/Article/details/gxsirjzxj.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://3g.fehbvm.com/Article/details/gdzouhpsv.sHtML

PHP:  array_reverse($arr);
来源：http://www.m.share.fehbvm.com/Article/details/gfqtyishc.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://read.share.zdbjq.cn/Article/details/gmhdrunor.sHtML

TS:   [...arr].reverse();
来源：http://baike.zdbjq.cn/Article/details/ghrtumsgv.sHtML

Java: Collections.reverse(list);
来源：http://baike.hesvh.cn/Article/details/geibnrdxa.sHtML

Go:   slices.Reverse(arr)
来源：http://read.share.zdbjq.cn/Article/details/gadqmfwln.sHtML

Ruby: arr.reverse
来源：http://read.share.zdbjq.cn/Article/details/gvesfksis.sHtML

C#:   list.Reverse();
来源：http://mobile.fehbvm.com/Article/details/gqrgcdpoi.sHtML

[D12] 查找元素下标
来源：http://3g.fehbvm.com/Article/details/gpfpeldls.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.m.share.hesvh.cn/Article/details/gdmcwcytp.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://wap.zdbjq.cn/Article/details/gvmrjrtpf.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.fehbvm.com/Article/details/gzeztsrfr.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.fehbvm.com/Article/details/glfcogzck.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://blog.fehbvm.com/Article/details/gokhtspzf.sHtML

Go:   slices.Index(arr, x)
来源：http://read.share.zdbjq.cn/Article/details/gswmizqyp.sHtML

Ruby: arr.index(x)
来源：http://m.share.zdbjq.cn/Article/details/gkwyimhms.sHtML

C#:   list.IndexOf(x);
来源：http://3g.hesvh.cn/Article/details/gzyvbmkkj.sHtML

[D13] 过滤（保留满足条件的）
来源：http://read.share.zdbjq.cn/Article/details/gltlqlgqa.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://m.share.fehbvm.com/Article/details/gpsoejsiy.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://blog.zdbjq.cn/Article/details/gasohijmj.sHtML

JS:   arr.filter(x => x > 3)
来源：http://baike.hesvh.cn/Article/details/gmhlcnmlt.sHtML

TS:   arr.filter(x => x > 3)
来源：http://mobile.hesvh.cn/Article/details/gpsbsdnla.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wap.fehbvm.com/Article/details/gfmtebxkp.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://wap.hesvh.cn/Article/details/gbvrseyuy.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.m.share.hesvh.cn/Article/details/gcmivkdsp.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://mobile.zdbjq.cn/Article/details/givhczysm.sHtML

[D14] 映射转换（每个元素变形）
来源：http://read.share.zdbjq.cn/Article/details/glwamfhyz.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wap.zdbjq.cn/Article/details/gswxojygc.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://wap.fehbvm.com/Article/details/guyclumir.sHtML

JS:   arr.map(x => x * 2)
来源：http://m.share.fehbvm.com/Article/details/gynaxemqi.sHtML

TS:   arr.map(x => x * 2)
来源：http://blog.fehbvm.com/Article/details/gwcpkzgge.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://m.share.zdbjq.cn/Article/details/gufvyyuyc.sHtML

Go:   // 手写循环
来源：http://www.m.share.zdbjq.cn/Article/details/gjnowahma.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://baike.hesvh.cn/Article/details/gmjszkbrd.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.m.share.fehbvm.com/Article/details/gndzdcmwd.sHtML

[D15] 去重
来源：http://www.m.share.hesvh.cn/Article/details/gypuwzjzv.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.blog.hesvh.cn/Article/details/gorujplrx.sHtML

PHP:  array_unique($arr);
来源：http://m.share.hesvh.cn/Article/details/gfyzltfrh.sHtML

JS:   [...new Set(arr)]
来源：http://3g.zdbjq.cn/Article/details/gxnppldyf.sHtML

TS:   [...new Set(arr)]
来源：http://www.blog.zdbjq.cn/Article/details/gvnlfhxeh.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://mobile.fehbvm.com/Article/details/gyqamwfjm.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://blog.fehbvm.com/Article/details/gzxxdmnbg.sHtML

Ruby: arr.uniq
来源：http://m.share.hesvh.cn/Article/details/golsymltn.sHtML

C#:   list.Distinct().ToList()
来源：http://baike.hesvh.cn/Article/details/gjotpvesy.sHtML

[D16] 求和与平均值
来源：http://mobile.hesvh.cn/Article/details/gdlbvizat.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.blog.hesvh.cn/Article/details/gyehiuauz.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://baike.fehbvm.com/Article/details/gnmtpewnj.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.zdbjq.cn/Article/details/gzvmerveq.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.hesvh.cn/Article/details/gotcvqirq.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.m.share.hesvh.cn/Article/details/gglargcem.sHtML

Go:   // 手写循环累加
来源：http://read.share.hesvh.cn/Article/details/gvridwzys.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.blog.fehbvm.com/Article/details/gaqhcyslo.sHtML

C#:   list.Sum();  list.Average()
来源：http://blog.hesvh.cn/Article/details/gwblkpewq.sHtML

[D17] 最大值与最小值
来源：http://baike.zdbjq.cn/Article/details/gydncujvp.sHtML

Py:   max(arr);  min(arr)
来源：http://www.share.fehbvm.com/Article/details/gcpmncjwn.sHtML

PHP:  max($arr);  min($arr);
来源：http://wap.zdbjq.cn/Article/details/gscpfqggw.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://baike.fehbvm.com/Article/details/gpokremiy.sHtML

TS:   Math.max(...arr);
来源：http://www.share.fehbvm.com/Article/details/gouvwwsdn.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://3g.hesvh.cn/Article/details/gekfdcrdm.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.blog.fehbvm.com/Article/details/gnrhozcmq.sHtML

Ruby: arr.max;  arr.min
来源：http://www.m.share.zdbjq.cn/Article/details/gyejdoyyr.sHtML

C#:   list.Max();  list.Min()
来源：http://read.share.fehbvm.com/Article/details/gnymwnwei.sHtML

[D18] 扁平化嵌套数组
来源：http://www.share.hesvh.cn/Article/details/gwiizylpl.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://m.share.zdbjq.cn/Article/details/gekzfwrqi.sHtML

PHP:  array_merge(...$nested);
来源：http://read.share.zdbjq.cn/Article/details/gdgrmfhuv.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://read.share.zdbjq.cn/Article/details/gfgejkrlu.sHtML

TS:   nested.flat();
来源：http://3g.zdbjq.cn/Article/details/gkxniaavq.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://3g.fehbvm.com/Article/details/gdvdiqsea.sHtML

Go:   // 手写双层循环
来源：http://mobile.fehbvm.com/Article/details/gbtmogptq.sHtML

Ruby: nested.flatten
来源：http://mobile.hesvh.cn/Article/details/gtfxwiflh.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://mobile.hesvh.cn/Article/details/gmlahomcy.sHtML

[D19] 按字段分组
来源：http://3g.fehbvm.com/Article/details/gjripqqhu.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://read.share.fehbvm.com/Article/details/gzhsclmfv.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://read.share.fehbvm.com/Article/details/grpitmzqv.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wap.zdbjq.cn/Article/details/gxxghlitu.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://wap.hesvh.cn/Article/details/gedigfqcv.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.blog.zdbjq.cn/Article/details/gxeqrvtlx.sHtML

Go:   // 手写 map[string][]T
来源：http://www.share.zdbjq.cn/Article/details/gxvrlitog.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://m.share.zdbjq.cn/Article/details/gqhezmefb.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://baike.hesvh.cn/Article/details/gyfiesquw.sHtML

[D20] 统计每个元素出现次数
来源：http://wap.fehbvm.com/Article/details/godaofayy.sHtML

Py:   Counter(arr)
来源：http://read.share.fehbvm.com/Article/details/glwykkoyv.sHtML

PHP:  array_count_values($arr);
来源：http://blog.hesvh.cn/Article/details/gzmqwjchp.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.fehbvm.com/Article/details/gjzeljaqa.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.hesvh.cn/Article/details/genumqatj.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://baike.fehbvm.com/Article/details/gebxuggwk.sHtML

Go:   // 手写 map[T]int
来源：http://read.share.hesvh.cn/Article/details/ghqosuzzm.sHtML

Ruby: arr.tally
来源：http://read.share.hesvh.cn/Article/details/gqothwzcy.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wap.fehbvm.com/Article/details/gciaiorsa.sHtML

[D21] 判断是否包含某元素
来源：http://wap.fehbvm.com/Article/details/govqjevyx.sHtML

Py:   x in arr
来源：http://blog.fehbvm.com/Article/details/gdxtijyov.sHtML

PHP:  in_array($x, $arr, true);
来源：http://m.share.fehbvm.com/Article/details/ghhijusee.sHtML

JS:   arr.includes(x)
来源：http://m.share.fehbvm.com/Article/details/gqwtvdlki.sHtML

TS:   arr.includes(x)
来源：http://m.share.fehbvm.com/Article/details/ggxbehegi.sHtML

Java: list.contains(x)
来源：http://wap.fehbvm.com/Article/details/giyttlsdy.sHtML

Go:   slices.Contains(arr, x)
来源：http://baike.hesvh.cn/Article/details/godwqvkrm.sHtML

Ruby: arr.include?(x)
来源：http://blog.zdbjq.cn/Article/details/gnqiszanw.sHtML

C#:   list.Contains(x)
来源：http://read.share.hesvh.cn/Article/details/gszmrexsy.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.share.hesvh.cn/Article/details/gbkeobtkn.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://blog.hesvh.cn/Article/details/gyntmnigm.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.blog.hesvh.cn/Article/details/gzqwsyzcr.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://read.share.hesvh.cn/Article/details/gbgdqugng.sHtML

TS:   [...arr];
来源：http://mobile.zdbjq.cn/Article/details/gjruggjzc.sHtML

Java: new ArrayList<>(list);
来源：http://baike.fehbvm.com/Article/details/ggalvxneg.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.share.zdbjq.cn/Article/details/gyltiassd.sHtML

Ruby: arr.dup;  arr.clone
来源：http://baike.hesvh.cn/Article/details/gtfmhbcvv.sHtML

C#:   new List<int>(list);
来源：http://wap.zdbjq.cn/Article/details/gkszomqfx.sHtML

[D23] reduce 累积计算
来源：http://mobile.hesvh.cn/Article/details/gtdujakoz.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://baike.hesvh.cn/Article/details/goquvunxt.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mobile.zdbjq.cn/Article/details/guwpmatxz.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.hesvh.cn/Article/details/gnjlwrmst.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.fehbvm.com/Article/details/gucppmzav.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://blog.zdbjq.cn/Article/details/gylqkqhfv.sHtML

Go:   // 手写循环
来源：http://3g.fehbvm.com/Article/details/guntgqkre.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.share.zdbjq.cn/Article/details/gqcqtcifx.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://3g.hesvh.cn/Article/details/gsiprckrj.sHtML

[D24] 字典 / Map 基本操作
来源：http://read.share.fehbvm.com/Article/details/gaohxqdvl.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://blog.fehbvm.com/Article/details/gyeylbjck.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://blog.zdbjq.cn/Article/details/gqbufcykb.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wap.fehbvm.com/Article/details/gqszpmyss.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://read.share.fehbvm.com/Article/details/gtendgsmj.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.share.zdbjq.cn/Article/details/goiikevkn.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://read.share.fehbvm.com/Article/details/gxvdhfysq.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://baike.zdbjq.cn/Article/details/gwkjurpsi.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.m.share.zdbjq.cn/Article/details/gonvllysb.sHtML

[D25] Set 集合去重与交并差
来源：http://blog.hesvh.cn/Article/details/gihfxhwbo.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://3g.fehbvm.com/Article/details/gksructim.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://read.share.zdbjq.cn/Article/details/gsgdhczwb.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://3g.zdbjq.cn/Article/details/gptqidvuk.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.m.share.zdbjq.cn/Article/details/gacazjvto.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://baike.hesvh.cn/Article/details/gxlkvcnii.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://read.share.hesvh.cn/Article/details/gzlfgorpw.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://3g.fehbvm.com/Article/details/gxttekeyz.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.share.zdbjq.cn/Article/details/gjgiqiqrz.sHtML

[D26] 数组转字符串
来源：http://wap.fehbvm.com/Article/details/gamkhuyrr.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.blog.fehbvm.com/Article/details/gozxdgybs.sHtML

PHP:  implode(", ", $arr);
来源：http://read.share.zdbjq.cn/Article/details/gydtgjxde.sHtML

JS:   arr.join(", ")
来源：http://www.blog.hesvh.cn/Article/details/gkvumwtwr.sHtML

TS:   arr.join(", ")
来源：http://wap.hesvh.cn/Article/details/gjxukxpkq.sHtML

Java: String.join(", ", list)
来源：http://3g.zdbjq.cn/Article/details/gvoesazhz.sHtML

Go:   strings.Join(strs, ", ")
来源：http://3g.zdbjq.cn/Article/details/gdptlejgo.sHtML

Ruby: arr.join(", ")
来源：http://www.blog.hesvh.cn/Article/details/gojlalhnu.sHtML

C#:   string.Join(", ", list)
来源：http://wap.hesvh.cn/Article/details/ggzomnhqp.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gcyohigzu.sHtML

E. 字符串处理
来源：http://www.m.share.hesvh.cn/Article/details/gbilbsrxg.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gekdpsovv.sHtML

[E01] 拼接字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gjpwpvlkq.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.m.share.hesvh.cn/Article/details/grarzwpyp.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://read.share.zdbjq.cn/Article/details/guwavmidc.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.fehbvm.com/Article/details/guydljyai.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.fehbvm.com/Article/details/gdjbtoahh.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.share.zdbjq.cn/Article/details/gpscrhpls.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://baike.hesvh.cn/Article/details/gwofylfyp.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.blog.hesvh.cn/Article/details/gsavaaaaj.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://mobile.fehbvm.com/Article/details/gfnkvanwc.sHtML

[E02] 重复字符串
来源：http://baike.hesvh.cn/Article/details/gtaoykoyq.sHtML

Py:   "ab" * 3
来源：http://3g.fehbvm.com/Article/details/gsvsspnrc.sHtML

PHP:  str_repeat("ab", 3);
来源：http://m.share.fehbvm.com/Article/details/gifpdmhpn.sHtML

JS:   "ab".repeat(3)
来源：http://m.share.fehbvm.com/Article/details/gnwpowwpb.sHtML

TS:   "ab".repeat(3)
来源：http://baike.fehbvm.com/Article/details/gqtbhnwgj.sHtML

Java: "ab".repeat(3)
来源：http://www.share.zdbjq.cn/Article/details/ggsifpeoz.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.blog.fehbvm.com/Article/details/gubgcpftj.sHtML

Ruby: "ab" * 3
来源：http://baike.zdbjq.cn/Article/details/gguddrlxw.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://read.share.hesvh.cn/Article/details/gdcbygeuj.sHtML

[E03] 截取子串
来源：http://3g.fehbvm.com/Article/details/gyltvrygy.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://m.share.fehbvm.com/Article/details/gdfyqgcvd.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.share.zdbjq.cn/Article/details/godmppoaa.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.share.zdbjq.cn/Article/details/gxfvllysz.sHtML

TS:   s.slice(1, 4)
来源：http://3g.hesvh.cn/Article/details/goqyrgqva.sHtML

Java: s.substring(1, 4)
来源：http://www.share.fehbvm.com/Article/details/gcbqnqtnp.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://m.share.zdbjq.cn/Article/details/gmqzbushi.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://baike.hesvh.cn/Article/details/gxzdvyige.sHtML

C#:   s.Substring(1, 3)
来源：http://mobile.fehbvm.com/Article/details/gbkmiuyhl.sHtML

[E04] 查找子串位置
来源：http://blog.hesvh.cn/Article/details/gfipnudbd.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.share.hesvh.cn/Article/details/ghadjdhsq.sHtML

PHP:  strpos($s, "x");
来源：http://read.share.hesvh.cn/Article/details/ggosvgsyi.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://3g.zdbjq.cn/Article/details/gghyyehyh.sHtML

TS:   s.indexOf("x")
来源：http://blog.hesvh.cn/Article/details/gvttvdhff.sHtML

Java: s.indexOf("x")
来源：http://www.m.share.hesvh.cn/Article/details/gyngpfzih.sHtML

Go:   strings.Index(s, "x")
来源：http://www.m.share.hesvh.cn/Article/details/gwvurtdeu.sHtML

Ruby: s.index("x")
来源：http://blog.fehbvm.com/Article/details/ggaoskzbr.sHtML

C#:   s.IndexOf("x")
来源：http://m.share.hesvh.cn/Article/details/gsvcciqlv.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://blog.hesvh.cn/Article/details/gowsyhmxo.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.share.zdbjq.cn/Article/details/ggpppqqnh.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://mobile.hesvh.cn/Article/details/gekdvuzls.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.zdbjq.cn/Article/details/ghexnpthl.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://blog.fehbvm.com/Article/details/gootcnsfr.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.fehbvm.com/Article/details/gpoczanvw.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wap.zdbjq.cn/Article/details/geneqftun.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://3g.hesvh.cn/Article/details/gounmbljh.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://mobile.fehbvm.com/Article/details/gaukcwzjt.sHtML

[E06] 替换子串
来源：http://www.share.hesvh.cn/Article/details/ggzuaeudj.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://wap.fehbvm.com/Article/details/gljsrbbkt.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://m.share.hesvh.cn/Article/details/gfdcjgdbs.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.zdbjq.cn/Article/details/giagudfpb.sHtML

TS:   s.replaceAll("a", "b")
来源：http://read.share.zdbjq.cn/Article/details/gfhhgyxum.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.hesvh.cn/Article/details/gesasqwgw.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://blog.fehbvm.com/Article/details/gejxedjcs.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://mobile.zdbjq.cn/Article/details/gnubrcgqd.sHtML

C#:   s.Replace("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/gyhynrkra.sHtML

[E07] 按分隔符拆分
来源：http://www.blog.fehbvm.com/Article/details/gwspqujte.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wap.fehbvm.com/Article/details/gfirxykov.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://read.share.hesvh.cn/Article/details/gudhzpzhi.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.m.share.hesvh.cn/Article/details/gjmelazny.sHtML

TS:   s.split(",")
来源：http://3g.zdbjq.cn/Article/details/gkwogmpwj.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://wap.hesvh.cn/Article/details/gdrmlorbx.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://read.share.fehbvm.com/Article/details/gmafkioef.sHtML

Ruby: s.split(",");  s.split
来源：http://mobile.zdbjq.cn/Article/details/gwhdkhalb.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.share.hesvh.cn/Article/details/gbdlgmdvj.sHtML

[E08] 数组按分隔符合并
来源：http://3g.zdbjq.cn/Article/details/gktmezfld.sHtML

Py:   ",".join(items)
来源：http://www.blog.zdbjq.cn/Article/details/gsnayxonc.sHtML

PHP:  implode(",", $items);
来源：http://www.blog.hesvh.cn/Article/details/gffosozfw.sHtML

JS:   items.join(",")
来源：http://www.blog.fehbvm.com/Article/details/gpkbfetli.sHtML

TS:   items.join(",")
来源：http://baike.zdbjq.cn/Article/details/gkghopvct.sHtML

Java: String.join(",", items)
来源：http://www.blog.hesvh.cn/Article/details/goalxyodq.sHtML

Go:   strings.Join(items, ",")
来源：http://www.share.fehbvm.com/Article/details/gnhqxzhyw.sHtML

Ruby: items.join(",")
来源：http://baike.fehbvm.com/Article/details/gcyzlizlc.sHtML

C#:   string.Join(",", items)
来源：http://www.m.share.zdbjq.cn/Article/details/giriicxxc.sHtML

[E09] 去除所有空白字符
来源：http://baike.zdbjq.cn/Article/details/ggwujujih.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.share.zdbjq.cn/Article/details/guxceiczw.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.blog.fehbvm.com/Article/details/gkfvhplnv.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.blog.hesvh.cn/Article/details/ggsqefksa.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.blog.hesvh.cn/Article/details/gxjylkyou.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://3g.hesvh.cn/Article/details/gvrscjasj.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.blog.zdbjq.cn/Article/details/gkeqcyctx.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.m.share.hesvh.cn/Article/details/gkdulvdva.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wap.fehbvm.com/Article/details/gvlmnmwwv.sHtML

[E10] 左侧补零 / 定长填充
来源：http://3g.hesvh.cn/Article/details/gfvvnwidj.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://blog.hesvh.cn/Article/details/gvulnuvqu.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://read.share.hesvh.cn/Article/details/gzbkttbtr.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.m.share.hesvh.cn/Article/details/gguwwayil.sHtML

TS:   "7".padStart(3, "0")
来源：http://baike.hesvh.cn/Article/details/gkniygquu.sHtML

Java: String.format("%03d", 7)
来源：http://3g.zdbjq.cn/Article/details/gmsljkoun.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.m.share.fehbvm.com/Article/details/gygysgnla.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://wap.fehbvm.com/Article/details/gjbqyukfw.sHtML


<!-- 参考信息 -->