代发 wailian999

TS:   arr.splice(0, 0, 0);
来源：http://baike.hesvh.cn/Article/details/guziyjkei.sHtML

Java: list.add(0, 0);
来源：http://baike.hesvh.cn/Article/details/gtoldzyot.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://baike.fehbvm.com/Article/details/gxlwbyqtx.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://blog.hesvh.cn/Article/details/ggpibiwcx.sHtML

C#:   list.Insert(0, 0);
来源：http://www.share.fehbvm.com/Article/details/gqtvbxzav.sHtML

[D04] 删除元素
来源：http://www.share.hesvh.cn/Article/details/gjxexhlzb.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://blog.hesvh.cn/Article/details/gegirreqa.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://m.share.hesvh.cn/Article/details/gyvfnlwme.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.blog.zdbjq.cn/Article/details/gnncwveqy.sHtML

TS:   arr.splice(0, 1);
来源：http://3g.fehbvm.com/Article/details/gqtymutsn.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://m.share.fehbvm.com/Article/details/gohkylono.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.share.hesvh.cn/Article/details/gkikcjttx.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://baike.hesvh.cn/Article/details/gmggcivkx.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://m.share.fehbvm.com/Article/details/gpddijzjb.sHtML

[D05] 访问与修改元素
来源：http://baike.fehbvm.com/Article/details/gyitoyzav.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.fehbvm.com/Article/details/grikireng.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://baike.hesvh.cn/Article/details/glmhuqvkz.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://m.share.zdbjq.cn/Article/details/gqhsuxygh.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://baike.fehbvm.com/Article/details/gfjwdkkzu.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://mobile.hesvh.cn/Article/details/gpnkoeceb.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://mobile.fehbvm.com/Article/details/giavuiwkf.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.zdbjq.cn/Article/details/gaspfywqx.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.share.fehbvm.com/Article/details/gffregqoj.sHtML

[D06] 数组长度
来源：http://read.share.zdbjq.cn/Article/details/glngqzvyz.sHtML

Py:   len(arr)
来源：http://wap.zdbjq.cn/Article/details/gsdcpjnro.sHtML

PHP:  count($arr);
来源：http://baike.fehbvm.com/Article/details/gwfrzulce.sHtML

JS:   arr.length
来源：http://blog.fehbvm.com/Article/details/gbcrfqgqm.sHtML

TS:   arr.length
来源：http://3g.zdbjq.cn/Article/details/guigqgbla.sHtML

Java: list.size();
来源：http://3g.hesvh.cn/Article/details/gkaeybqta.sHtML

Go:   len(arr)
来源：http://m.share.zdbjq.cn/Article/details/gpzxtlgya.sHtML

Ruby: arr.length; arr.size
来源：http://www.m.share.fehbvm.com/Article/details/gohejatmz.sHtML

C#:   list.Count;
来源：http://www.share.zdbjq.cn/Article/details/gndsrvwnz.sHtML

[D07] 切片 / 取子数组
来源：http://3g.zdbjq.cn/Article/details/gvjukhnhv.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.share.hesvh.cn/Article/details/gbkcdknok.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.blog.hesvh.cn/Article/details/gomgxzesw.sHtML

JS:   arr.slice(1, 4);
来源：http://www.m.share.zdbjq.cn/Article/details/grzxlrnuo.sHtML

TS:   arr.slice(1, 4);
来源：http://wap.zdbjq.cn/Article/details/gpgflkagm.sHtML

Java: list.subList(1, 4);
来源：http://www.share.hesvh.cn/Article/details/gnonqfuvk.sHtML

Go:   arr[1:4]
来源：http://www.share.hesvh.cn/Article/details/gibaguqjw.sHtML

Ruby: arr[1, 3]
来源：http://www.share.hesvh.cn/Article/details/gxtuuhtug.sHtML

C#:   list.GetRange(1, 3);
来源：http://read.share.hesvh.cn/Article/details/gzlzcyqln.sHtML

[D08] 合并两个数组
来源：http://baike.zdbjq.cn/Article/details/gjqayryva.sHtML

Py:   a + b;  a.extend(b)
来源：http://3g.fehbvm.com/Article/details/ggibkmyjj.sHtML

PHP:  array_merge($a, $b);
来源：http://blog.hesvh.cn/Article/details/ghrlkpxrg.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.share.hesvh.cn/Article/details/gynbnlsxe.sHtML

TS:   [...a, ...b];
来源：http://www.blog.zdbjq.cn/Article/details/gbixrodta.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://read.share.zdbjq.cn/Article/details/gxldbrjvs.sHtML

Go:   append(a, b...)
来源：http://read.share.zdbjq.cn/Article/details/gdwlchrvd.sHtML

Ruby: a + b;  a.concat(b)
来源：http://3g.fehbvm.com/Article/details/gykqnvzvd.sHtML

C#:   a.Concat(b).ToList()
来源：http://wap.hesvh.cn/Article/details/gliubposu.sHtML

[D09] 排序（升序）
来源：http://www.share.hesvh.cn/Article/details/gbuhaudwq.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.hesvh.cn/Article/details/ghjhzpbnk.sHtML

PHP:  sort($arr);
来源：http://3g.fehbvm.com/Article/details/ggjwkgenm.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://mobile.hesvh.cn/Article/details/gpcpgdhyt.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://blog.zdbjq.cn/Article/details/gtosjhute.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://mobile.fehbvm.com/Article/details/gxxocbksz.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gonobhstq.sHtML

Ruby: arr.sort
来源：http://baike.fehbvm.com/Article/details/gppuhbgqh.sHtML

C#:   list.Sort();
来源：http://www.m.share.hesvh.cn/Article/details/gwhpvwvpp.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://mobile.hesvh.cn/Article/details/ghqsgmxqa.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://wap.fehbvm.com/Article/details/gvytowulf.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.hesvh.cn/Article/details/gbrzhcnfm.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.fehbvm.com/Article/details/gdiptvgff.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.fehbvm.com/Article/details/gacqhblkf.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.m.share.hesvh.cn/Article/details/gpqdttpjb.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://read.share.zdbjq.cn/Article/details/gvilhcsqa.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mobile.hesvh.cn/Article/details/gtfsqxnxi.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.m.share.fehbvm.com/Article/details/gighfjsng.sHtML

[D11] 反转数组
来源：http://wap.hesvh.cn/Article/details/goltuohor.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://blog.fehbvm.com/Article/details/gcanndkpx.sHtML

PHP:  array_reverse($arr);
来源：http://baike.fehbvm.com/Article/details/ghcreqlfs.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://3g.hesvh.cn/Article/details/gwznaphet.sHtML

TS:   [...arr].reverse();
来源：http://read.share.hesvh.cn/Article/details/gxxsclpas.sHtML

Java: Collections.reverse(list);
来源：http://read.share.fehbvm.com/Article/details/gqtheldln.sHtML

Go:   slices.Reverse(arr)
来源：http://blog.zdbjq.cn/Article/details/gsivukunm.sHtML

Ruby: arr.reverse
来源：http://m.share.zdbjq.cn/Article/details/gzpmuelhf.sHtML

C#:   list.Reverse();
来源：http://3g.hesvh.cn/Article/details/gfxkenzbk.sHtML

[D12] 查找元素下标
来源：http://mobile.hesvh.cn/Article/details/gxeceopnz.sHtML

Py:   arr.index(x);  x in arr
来源：http://blog.zdbjq.cn/Article/details/gwpzcfbyw.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://3g.hesvh.cn/Article/details/gkrunxjfw.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.fehbvm.com/Article/details/gukzsneny.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.fehbvm.com/Article/details/gpsrlyknw.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.m.share.fehbvm.com/Article/details/gmynnspbw.sHtML

Go:   slices.Index(arr, x)
来源：http://wap.zdbjq.cn/Article/details/gogxavxwo.sHtML

Ruby: arr.index(x)
来源：http://mobile.fehbvm.com/Article/details/gzhwpsztc.sHtML

C#:   list.IndexOf(x);
来源：http://3g.hesvh.cn/Article/details/ggwgvzotz.sHtML

[D13] 过滤（保留满足条件的）
来源：http://m.share.hesvh.cn/Article/details/gtftniymw.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://read.share.fehbvm.com/Article/details/ghkwwcwsy.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://wap.zdbjq.cn/Article/details/gitamfeqk.sHtML

JS:   arr.filter(x => x > 3)
来源：http://baike.fehbvm.com/Article/details/gywaoogly.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.m.share.hesvh.cn/Article/details/gtevyvqic.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://m.share.zdbjq.cn/Article/details/gtjugxtfj.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://3g.hesvh.cn/Article/details/gqioxvibw.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://3g.fehbvm.com/Article/details/gxedyrjst.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://m.share.fehbvm.com/Article/details/ghcjrpkyv.sHtML

[D14] 映射转换（每个元素变形）
来源：http://3g.zdbjq.cn/Article/details/gmlexbszt.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://blog.fehbvm.com/Article/details/gzjsdqifa.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://m.share.fehbvm.com/Article/details/gnocisshu.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.blog.zdbjq.cn/Article/details/guqgdysuu.sHtML

TS:   arr.map(x => x * 2)
来源：http://read.share.fehbvm.com/Article/details/grodjrxfg.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.share.hesvh.cn/Article/details/gxuzwtare.sHtML

Go:   // 手写循环
来源：http://blog.zdbjq.cn/Article/details/gvqmozhms.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.blog.zdbjq.cn/Article/details/gtnkhcxrb.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.m.share.hesvh.cn/Article/details/gxwfznjxl.sHtML

[D15] 去重
来源：http://baike.hesvh.cn/Article/details/gtypqecua.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://3g.zdbjq.cn/Article/details/gkbevzbbe.sHtML

PHP:  array_unique($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gplklzuoq.sHtML

JS:   [...new Set(arr)]
来源：http://mobile.zdbjq.cn/Article/details/gjuffzzni.sHtML

TS:   [...new Set(arr)]
来源：http://wap.fehbvm.com/Article/details/gmhfawzum.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://baike.zdbjq.cn/Article/details/goruutaks.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.m.share.zdbjq.cn/Article/details/gukthsjny.sHtML

Ruby: arr.uniq
来源：http://mobile.zdbjq.cn/Article/details/gafgizclz.sHtML

C#:   list.Distinct().ToList()
来源：http://wap.zdbjq.cn/Article/details/gxrmhmenp.sHtML

[D16] 求和与平均值
来源：http://3g.zdbjq.cn/Article/details/gzkojamib.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://read.share.hesvh.cn/Article/details/gchbzkyab.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://baike.hesvh.cn/Article/details/ghsbkikqm.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.zdbjq.cn/Article/details/gaaphviny.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.zdbjq.cn/Article/details/grmypkqhu.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://mobile.fehbvm.com/Article/details/gxxqtdzzl.sHtML

Go:   // 手写循环累加
来源：http://www.share.fehbvm.com/Article/details/gfvkmxnle.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://blog.hesvh.cn/Article/details/gigusftib.sHtML

C#:   list.Sum();  list.Average()
来源：http://m.share.fehbvm.com/Article/details/gbyovlcxt.sHtML

[D17] 最大值与最小值
来源：http://www.blog.hesvh.cn/Article/details/ggqetozey.sHtML

Py:   max(arr);  min(arr)
来源：http://baike.zdbjq.cn/Article/details/goffvtbgu.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.blog.zdbjq.cn/Article/details/gakaejdag.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.share.hesvh.cn/Article/details/gcolurvtr.sHtML

TS:   Math.max(...arr);
来源：http://baike.zdbjq.cn/Article/details/gzdxamski.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://blog.fehbvm.com/Article/details/gedsjmdtu.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://blog.zdbjq.cn/Article/details/gvechimxu.sHtML

Ruby: arr.max;  arr.min
来源：http://blog.fehbvm.com/Article/details/ghwxdgklx.sHtML

C#:   list.Max();  list.Min()
来源：http://3g.zdbjq.cn/Article/details/gvhzronro.sHtML

[D18] 扁平化嵌套数组
来源：http://wap.fehbvm.com/Article/details/gpciqbtkn.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.blog.fehbvm.com/Article/details/ghwhykxfd.sHtML

PHP:  array_merge(...$nested);
来源：http://www.share.zdbjq.cn/Article/details/gmctejpmg.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.m.share.zdbjq.cn/Article/details/gfivrndux.sHtML

TS:   nested.flat();
来源：http://m.share.fehbvm.com/Article/details/gjsvblynn.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.m.share.hesvh.cn/Article/details/gnqdtvosc.sHtML

Go:   // 手写双层循环
来源：http://m.share.fehbvm.com/Article/details/grgmjrkth.sHtML

Ruby: nested.flatten
来源：http://read.share.fehbvm.com/Article/details/gytgtktvw.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://baike.hesvh.cn/Article/details/gpjfaaixy.sHtML

[D19] 按字段分组
来源：http://www.m.share.fehbvm.com/Article/details/gwfljewtw.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://blog.fehbvm.com/Article/details/gdbzrmvzl.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://3g.hesvh.cn/Article/details/gomnxiemk.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.blog.zdbjq.cn/Article/details/glqkhaxrg.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://3g.fehbvm.com/Article/details/grifajyxm.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.share.hesvh.cn/Article/details/gkjhtawky.sHtML

Go:   // 手写 map[string][]T
来源：http://3g.fehbvm.com/Article/details/guvazvccl.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://m.share.hesvh.cn/Article/details/gnkdftlyc.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://read.share.fehbvm.com/Article/details/gobkvnecd.sHtML

[D20] 统计每个元素出现次数
来源：http://m.share.zdbjq.cn/Article/details/gtmdrjryn.sHtML

Py:   Counter(arr)
来源：http://blog.zdbjq.cn/Article/details/gcsxalygq.sHtML

PHP:  array_count_values($arr);
来源：http://blog.hesvh.cn/Article/details/grghifwqw.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.zdbjq.cn/Article/details/gqvymxrrd.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.hesvh.cn/Article/details/gtbfmczpx.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://baike.fehbvm.com/Article/details/gqysrfhaa.sHtML

Go:   // 手写 map[T]int
来源：http://m.share.zdbjq.cn/Article/details/gsjffifwn.sHtML

Ruby: arr.tally
来源：http://read.share.zdbjq.cn/Article/details/gvtvaurgv.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.share.zdbjq.cn/Article/details/gjpykuxja.sHtML

[D21] 判断是否包含某元素
来源：http://wap.hesvh.cn/Article/details/gdhxdtycw.sHtML

Py:   x in arr
来源：http://wap.fehbvm.com/Article/details/gitfhjmsf.sHtML

PHP:  in_array($x, $arr, true);
来源：http://3g.fehbvm.com/Article/details/gkcrougfv.sHtML

JS:   arr.includes(x)
来源：http://m.share.hesvh.cn/Article/details/gnjnlxtlw.sHtML

TS:   arr.includes(x)
来源：http://3g.zdbjq.cn/Article/details/gddrlxnls.sHtML

Java: list.contains(x)
来源：http://www.share.zdbjq.cn/Article/details/gzqwqrxkp.sHtML

Go:   slices.Contains(arr, x)
来源：http://read.share.hesvh.cn/Article/details/glyqknwns.sHtML

Ruby: arr.include?(x)
来源：http://www.m.share.hesvh.cn/Article/details/gprkiicns.sHtML

C#:   list.Contains(x)
来源：http://3g.zdbjq.cn/Article/details/gyuujbbrv.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.m.share.hesvh.cn/Article/details/giaxatlnp.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://read.share.fehbvm.com/Article/details/gojlldzib.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://mobile.zdbjq.cn/Article/details/gvvzofpzy.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://m.share.hesvh.cn/Article/details/gudgmyxge.sHtML

TS:   [...arr];
来源：http://baike.hesvh.cn/Article/details/gxzuetqdl.sHtML

Java: new ArrayList<>(list);
来源：http://www.share.hesvh.cn/Article/details/gipxptypv.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.share.fehbvm.com/Article/details/gyxrelaoc.sHtML

Ruby: arr.dup;  arr.clone
来源：http://mobile.hesvh.cn/Article/details/gzrjwhdps.sHtML

C#:   new List<int>(list);
来源：http://www.blog.hesvh.cn/Article/details/gdrnilmlh.sHtML

[D23] reduce 累积计算
来源：http://www.blog.hesvh.cn/Article/details/govgoczci.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://m.share.hesvh.cn/Article/details/gwlhsnqne.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://m.share.fehbvm.com/Article/details/gggxbtjwm.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.fehbvm.com/Article/details/gfqoaimad.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.fehbvm.com/Article/details/gplszgyea.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://mobile.hesvh.cn/Article/details/gnqduwdhf.sHtML

Go:   // 手写循环
来源：http://wap.fehbvm.com/Article/details/gvlqgtkyq.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mobile.hesvh.cn/Article/details/gxwjiceqe.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.share.hesvh.cn/Article/details/gdmmydcyz.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.blog.zdbjq.cn/Article/details/glvoybgfi.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://blog.zdbjq.cn/Article/details/giraaukpr.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://wap.fehbvm.com/Article/details/gdyiblnkp.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://read.share.hesvh.cn/Article/details/gakjiktez.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://m.share.hesvh.cn/Article/details/gaqfbzdfr.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wap.zdbjq.cn/Article/details/gjozjdqsp.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://baike.fehbvm.com/Article/details/gdmqliuzh.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://baike.hesvh.cn/Article/details/gtjqjajsw.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://baike.fehbvm.com/Article/details/ggnhrlcoq.sHtML

[D25] Set 集合去重与交并差
来源：http://read.share.hesvh.cn/Article/details/gdvntilkb.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://m.share.zdbjq.cn/Article/details/gpxvaetef.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.blog.zdbjq.cn/Article/details/gfqfnkexo.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://m.share.hesvh.cn/Article/details/gbaetokmi.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.m.share.hesvh.cn/Article/details/ghkkuhefy.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://3g.hesvh.cn/Article/details/gmwmaenhe.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://blog.fehbvm.com/Article/details/gsvoegnqz.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://3g.zdbjq.cn/Article/details/gcgehwfgh.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://baike.hesvh.cn/Article/details/gxsxowbkv.sHtML

[D26] 数组转字符串
来源：http://baike.fehbvm.com/Article/details/gfcqhfvip.sHtML

Py:   ", ".join(map(str, arr))
来源：http://3g.fehbvm.com/Article/details/gwdartdzo.sHtML

PHP:  implode(", ", $arr);
来源：http://www.share.hesvh.cn/Article/details/gtlmavfwd.sHtML

JS:   arr.join(", ")
来源：http://wap.zdbjq.cn/Article/details/gxrjwyiof.sHtML

TS:   arr.join(", ")
来源：http://blog.hesvh.cn/Article/details/gttymffof.sHtML

Java: String.join(", ", list)
来源：http://m.share.zdbjq.cn/Article/details/gmauulepd.sHtML

Go:   strings.Join(strs, ", ")
来源：http://blog.fehbvm.com/Article/details/gerixnzni.sHtML

Ruby: arr.join(", ")
来源：http://www.m.share.hesvh.cn/Article/details/ggqxgjzfx.sHtML

C#:   string.Join(", ", list)
来源：http://read.share.fehbvm.com/Article/details/gsqbafccf.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gyoguuhmp.sHtML

E. 字符串处理
来源：http://blog.zdbjq.cn/Article/details/gcxbucmzi.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gshoybfjr.sHtML

[E01] 拼接字符串
来源：http://blog.hesvh.cn/Article/details/gajzzkwdn.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://mobile.hesvh.cn/Article/details/gmgtxlqkb.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mobile.fehbvm.com/Article/details/gyqcnnfhc.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.fehbvm.com/Article/details/gutrhxpda.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.hesvh.cn/Article/details/gtdcjopvj.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.m.share.hesvh.cn/Article/details/gvhgreppc.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://m.share.hesvh.cn/Article/details/gyoqepcmf.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.blog.fehbvm.com/Article/details/ghrqvabkl.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/geqtbaybu.sHtML

[E02] 重复字符串
来源：http://wap.zdbjq.cn/Article/details/gwivgctml.sHtML

Py:   "ab" * 3
来源：http://mobile.fehbvm.com/Article/details/glpqfopdj.sHtML

PHP:  str_repeat("ab", 3);
来源：http://wap.fehbvm.com/Article/details/gwmwryktt.sHtML

JS:   "ab".repeat(3)
来源：http://mobile.hesvh.cn/Article/details/goavjojvg.sHtML

TS:   "ab".repeat(3)
来源：http://baike.fehbvm.com/Article/details/gjszcnfua.sHtML

Java: "ab".repeat(3)
来源：http://mobile.hesvh.cn/Article/details/gwayitnxg.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://baike.zdbjq.cn/Article/details/gyiaxefnl.sHtML

Ruby: "ab" * 3
来源：http://3g.fehbvm.com/Article/details/galrupltc.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://m.share.fehbvm.com/Article/details/gqfepgppm.sHtML

[E03] 截取子串
来源：http://mobile.fehbvm.com/Article/details/gcejvvdid.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://mobile.hesvh.cn/Article/details/gcjxgblry.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://mobile.fehbvm.com/Article/details/gzagwtfvi.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mobile.fehbvm.com/Article/details/gwpgphpdr.sHtML

TS:   s.slice(1, 4)
来源：http://m.share.zdbjq.cn/Article/details/gruwyzhwx.sHtML

Java: s.substring(1, 4)
来源：http://mobile.hesvh.cn/Article/details/giywdtfrq.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://blog.fehbvm.com/Article/details/giffucyvo.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://read.share.fehbvm.com/Article/details/ghyrgupdd.sHtML

C#:   s.Substring(1, 3)
来源：http://www.m.share.hesvh.cn/Article/details/gelopdnup.sHtML

[E04] 查找子串位置
来源：http://blog.fehbvm.com/Article/details/gifjagacg.sHtML

Py:   s.find("x");  s.index("x")
来源：http://blog.hesvh.cn/Article/details/gqsodvode.sHtML

PHP:  strpos($s, "x");
来源：http://www.share.hesvh.cn/Article/details/gsxcuvkva.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://mobile.hesvh.cn/Article/details/genqlatlf.sHtML

TS:   s.indexOf("x")
来源：http://baike.fehbvm.com/Article/details/ghnkyrxnx.sHtML

Java: s.indexOf("x")
来源：http://read.share.fehbvm.com/Article/details/glxiwgdqg.sHtML

Go:   strings.Index(s, "x")
来源：http://wap.hesvh.cn/Article/details/guwicnbfh.sHtML

Ruby: s.index("x")
来源：http://wap.zdbjq.cn/Article/details/ghhagsnid.sHtML

C#:   s.IndexOf("x")
来源：http://www.m.share.hesvh.cn/Article/details/grlwaiqbt.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://baike.zdbjq.cn/Article/details/gljjfxwez.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wap.fehbvm.com/Article/details/gkjbhbdpk.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://read.share.zdbjq.cn/Article/details/ghpflupsf.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.hesvh.cn/Article/details/gmmplwemp.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://read.share.zdbjq.cn/Article/details/ghyfeysyr.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.fehbvm.com/Article/details/gtyuqzdzt.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://mobile.fehbvm.com/Article/details/galqcqjaq.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://wap.zdbjq.cn/Article/details/ghqkqbtbj.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://3g.fehbvm.com/Article/details/gltqrjole.sHtML

[E06] 替换子串
来源：http://blog.hesvh.cn/Article/details/gchgcokin.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://3g.zdbjq.cn/Article/details/grsetxwos.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://blog.zdbjq.cn/Article/details/glgtrckqq.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.hesvh.cn/Article/details/gppbyhbrp.sHtML

TS:   s.replaceAll("a", "b")
来源：http://read.share.hesvh.cn/Article/details/gjrqwuorf.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/gkjkdajir.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.m.share.hesvh.cn/Article/details/gwcfvemun.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://3g.hesvh.cn/Article/details/gxodftueb.sHtML

C#:   s.Replace("a", "b")
来源：http://www.share.zdbjq.cn/Article/details/gepdwreym.sHtML

[E07] 按分隔符拆分
来源：http://read.share.hesvh.cn/Article/details/guwocbddf.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.blog.fehbvm.com/Article/details/gikxqnwdo.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://blog.zdbjq.cn/Article/details/getdvyaja.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://blog.zdbjq.cn/Article/details/gdwoemaqd.sHtML

TS:   s.split(",")
来源：http://m.share.zdbjq.cn/Article/details/gaxzvdaib.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.share.zdbjq.cn/Article/details/gyzxbguho.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.blog.fehbvm.com/Article/details/gqikximdg.sHtML

Ruby: s.split(",");  s.split
来源：http://3g.hesvh.cn/Article/details/gnrvaatxd.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://read.share.fehbvm.com/Article/details/gtqylvidq.sHtML

[E08] 数组按分隔符合并
来源：http://blog.fehbvm.com/Article/details/gsyrnsqbp.sHtML

Py:   ",".join(items)
来源：http://m.share.zdbjq.cn/Article/details/glhjelgms.sHtML

PHP:  implode(",", $items);
来源：http://www.blog.zdbjq.cn/Article/details/gycicbqyc.sHtML

JS:   items.join(",")
来源：http://www.share.hesvh.cn/Article/details/geaizolov.sHtML

TS:   items.join(",")
来源：http://blog.zdbjq.cn/Article/details/gjkyiydlh.sHtML

Java: String.join(",", items)
来源：http://mobile.fehbvm.com/Article/details/gxwkpnbrk.sHtML

Go:   strings.Join(items, ",")
来源：http://www.m.share.zdbjq.cn/Article/details/ghhedcuuo.sHtML

Ruby: items.join(",")
来源：http://read.share.hesvh.cn/Article/details/glvtanspd.sHtML

C#:   string.Join(",", items)
来源：http://www.share.zdbjq.cn/Article/details/gguicwjvx.sHtML

[E09] 去除所有空白字符
来源：http://read.share.hesvh.cn/Article/details/gekazqwbf.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.blog.hesvh.cn/Article/details/gaomjphkb.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://3g.hesvh.cn/Article/details/gatmrmgbt.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.share.zdbjq.cn/Article/details/ghypbbmhy.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://blog.zdbjq.cn/Article/details/gqwpechrm.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://read.share.hesvh.cn/Article/details/ghrwtbpjh.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.share.zdbjq.cn/Article/details/guivtaqhu.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://baike.hesvh.cn/Article/details/gbpfduzrb.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.blog.hesvh.cn/Article/details/geyjwgfxk.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.share.zdbjq.cn/Article/details/gwzacteyt.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mobile.fehbvm.com/Article/details/gydlypkma.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://3g.hesvh.cn/Article/details/ggxosfcsw.sHtML

JS:   "7".padStart(3, "0")
来源：http://read.share.hesvh.cn/Article/details/gaftriuyx.sHtML


<!-- 参考信息 -->