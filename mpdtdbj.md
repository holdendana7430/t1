代发 wailian999

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://blog.fehbvm.com/Article/details/gmgapuske.sHtML

TS:   arr.splice(0, 1);
来源：http://read.share.hesvh.cn/Article/details/glfjrvpal.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://read.share.fehbvm.com/Article/details/giaikzxpc.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://3g.hesvh.cn/Article/details/gjyixvzsj.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mobile.zdbjq.cn/Article/details/gttyujqde.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.share.fehbvm.com/Article/details/goxriyevq.sHtML

[D05] 访问与修改元素
来源：http://www.blog.hesvh.cn/Article/details/gmxwbgngg.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.fehbvm.com/Article/details/girrolfiz.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://m.share.fehbvm.com/Article/details/ggsenmplo.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://read.share.hesvh.cn/Article/details/guvrarmoz.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://blog.zdbjq.cn/Article/details/gjvxazior.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://wap.zdbjq.cn/Article/details/gkxrsaizd.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://m.share.fehbvm.com/Article/details/gskbsqjoc.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.zdbjq.cn/Article/details/gaqqewvkg.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.share.zdbjq.cn/Article/details/gdgvxinan.sHtML

[D06] 数组长度
来源：http://wap.fehbvm.com/Article/details/grhytzhve.sHtML

Py:   len(arr)
来源：http://blog.zdbjq.cn/Article/details/gdmgikugo.sHtML

PHP:  count($arr);
来源：http://m.share.zdbjq.cn/Article/details/gulqolmwi.sHtML

JS:   arr.length
来源：http://mobile.zdbjq.cn/Article/details/gdpjqwoul.sHtML

TS:   arr.length
来源：http://www.blog.fehbvm.com/Article/details/gxwsdwupp.sHtML

Java: list.size();
来源：http://wap.zdbjq.cn/Article/details/gnvbhuzaa.sHtML

Go:   len(arr)
来源：http://baike.zdbjq.cn/Article/details/gwfudctau.sHtML

Ruby: arr.length; arr.size
来源：http://blog.zdbjq.cn/Article/details/gowzfeqzs.sHtML

C#:   list.Count;
来源：http://www.share.hesvh.cn/Article/details/gkjtodzzj.sHtML

[D07] 切片 / 取子数组
来源：http://m.share.fehbvm.com/Article/details/gcvivhdmr.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.m.share.zdbjq.cn/Article/details/gnzsrnwgn.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://mobile.hesvh.cn/Article/details/gfsxdmoyi.sHtML

JS:   arr.slice(1, 4);
来源：http://www.blog.zdbjq.cn/Article/details/goeqbmizj.sHtML

TS:   arr.slice(1, 4);
来源：http://www.m.share.zdbjq.cn/Article/details/ggvtwubak.sHtML

Java: list.subList(1, 4);
来源：http://www.share.hesvh.cn/Article/details/gsvrsilps.sHtML

Go:   arr[1:4]
来源：http://blog.fehbvm.com/Article/details/gnzhkgbnw.sHtML

Ruby: arr[1, 3]
来源：http://read.share.zdbjq.cn/Article/details/gjmxcgket.sHtML

C#:   list.GetRange(1, 3);
来源：http://blog.hesvh.cn/Article/details/glblhsfos.sHtML

[D08] 合并两个数组
来源：http://wap.hesvh.cn/Article/details/gqmiyjzlx.sHtML

Py:   a + b;  a.extend(b)
来源：http://blog.fehbvm.com/Article/details/gnxrnzvtm.sHtML

PHP:  array_merge($a, $b);
来源：http://m.share.hesvh.cn/Article/details/gfoeorwtd.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://mobile.hesvh.cn/Article/details/ggbjecsex.sHtML

TS:   [...a, ...b];
来源：http://m.share.hesvh.cn/Article/details/gpjdjrbqi.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.share.fehbvm.com/Article/details/gatuiseio.sHtML

Go:   append(a, b...)
来源：http://mobile.fehbvm.com/Article/details/gfdpjcltl.sHtML

Ruby: a + b;  a.concat(b)
来源：http://m.share.fehbvm.com/Article/details/gkybyxjzk.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.m.share.hesvh.cn/Article/details/gtotsxtvs.sHtML

[D09] 排序（升序）
来源：http://3g.zdbjq.cn/Article/details/gvzyapisf.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.zdbjq.cn/Article/details/gnbpcoxew.sHtML

PHP:  sort($arr);
来源：http://blog.zdbjq.cn/Article/details/gbzbbqxne.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.share.zdbjq.cn/Article/details/gmlcbffpc.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://blog.zdbjq.cn/Article/details/gssjbtmnz.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://read.share.fehbvm.com/Article/details/gsctulqqb.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://wap.hesvh.cn/Article/details/gaankahof.sHtML

Ruby: arr.sort
来源：http://blog.hesvh.cn/Article/details/gdxvmckjq.sHtML

C#:   list.Sort();
来源：http://m.share.hesvh.cn/Article/details/gknzevmwk.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://baike.zdbjq.cn/Article/details/gpybgoqpv.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.blog.hesvh.cn/Article/details/ggwwxarvf.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.hesvh.cn/Article/details/gmhjdfwey.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.hesvh.cn/Article/details/gihkkevgf.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.fehbvm.com/Article/details/gjyqmxqdk.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://wap.zdbjq.cn/Article/details/gyonzdivq.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.m.share.hesvh.cn/Article/details/gfnshoreb.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://baike.zdbjq.cn/Article/details/guzlqdrew.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://3g.fehbvm.com/Article/details/gwbczwfvu.sHtML

[D11] 反转数组
来源：http://wap.hesvh.cn/Article/details/gqpyvjcxe.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.m.share.fehbvm.com/Article/details/gksgmnifo.sHtML

PHP:  array_reverse($arr);
来源：http://mobile.hesvh.cn/Article/details/ggfftnvql.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://m.share.fehbvm.com/Article/details/gwfxqbxtf.sHtML

TS:   [...arr].reverse();
来源：http://www.blog.fehbvm.com/Article/details/gjfqpxffe.sHtML

Java: Collections.reverse(list);
来源：http://www.blog.hesvh.cn/Article/details/goeazvwmd.sHtML

Go:   slices.Reverse(arr)
来源：http://baike.zdbjq.cn/Article/details/grlxsgkaq.sHtML

Ruby: arr.reverse
来源：http://mobile.hesvh.cn/Article/details/glvjwjxur.sHtML

C#:   list.Reverse();
来源：http://3g.zdbjq.cn/Article/details/gaebzrgzs.sHtML

[D12] 查找元素下标
来源：http://baike.hesvh.cn/Article/details/gfjgvfmip.sHtML

Py:   arr.index(x);  x in arr
来源：http://mobile.hesvh.cn/Article/details/gedifgucc.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://wap.zdbjq.cn/Article/details/girashfas.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.zdbjq.cn/Article/details/gcthcxjow.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.hesvh.cn/Article/details/gcwjggjwo.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://blog.hesvh.cn/Article/details/gflmvzjja.sHtML

Go:   slices.Index(arr, x)
来源：http://3g.fehbvm.com/Article/details/gzkvecfcc.sHtML

Ruby: arr.index(x)
来源：http://www.share.hesvh.cn/Article/details/gktxzazpg.sHtML

C#:   list.IndexOf(x);
来源：http://www.share.zdbjq.cn/Article/details/gyfvjoswk.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.m.share.hesvh.cn/Article/details/govihyzep.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://3g.hesvh.cn/Article/details/gegjhulze.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://mobile.hesvh.cn/Article/details/gycfltktc.sHtML

JS:   arr.filter(x => x > 3)
来源：http://read.share.hesvh.cn/Article/details/gtliviiym.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.m.share.fehbvm.com/Article/details/gqpqvyksb.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mobile.hesvh.cn/Article/details/gfpcjyzdl.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mobile.fehbvm.com/Article/details/gfiiktnsc.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.blog.zdbjq.cn/Article/details/gohczpeet.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.blog.hesvh.cn/Article/details/gcpzczlev.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.m.share.hesvh.cn/Article/details/gfwqdzpwm.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.share.fehbvm.com/Article/details/getwkopyc.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.share.zdbjq.cn/Article/details/gekhyvxqi.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.blog.zdbjq.cn/Article/details/gjfoisefy.sHtML

TS:   arr.map(x => x * 2)
来源：http://blog.hesvh.cn/Article/details/goyfdubtd.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://wap.hesvh.cn/Article/details/glnuioofv.sHtML

Go:   // 手写循环
来源：http://wap.fehbvm.com/Article/details/gsdvqokeu.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://m.share.zdbjq.cn/Article/details/gmonmxcfe.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://wap.fehbvm.com/Article/details/gsvrywoup.sHtML

[D15] 去重
来源：http://www.m.share.zdbjq.cn/Article/details/gbvjsaxxu.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://3g.zdbjq.cn/Article/details/gdeemqbzg.sHtML

PHP:  array_unique($arr);
来源：http://www.blog.zdbjq.cn/Article/details/gxmlgpzgr.sHtML

JS:   [...new Set(arr)]
来源：http://m.share.fehbvm.com/Article/details/grhkmegyn.sHtML

TS:   [...new Set(arr)]
来源：http://wap.zdbjq.cn/Article/details/gvlrwbnny.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://read.share.fehbvm.com/Article/details/gfqhlqvny.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://wap.hesvh.cn/Article/details/goqnhvxsx.sHtML

Ruby: arr.uniq
来源：http://m.share.zdbjq.cn/Article/details/gvydzmjky.sHtML

C#:   list.Distinct().ToList()
来源：http://www.m.share.zdbjq.cn/Article/details/gnfmflqkr.sHtML

[D16] 求和与平均值
来源：http://www.blog.fehbvm.com/Article/details/gpptqjpmf.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wap.hesvh.cn/Article/details/gftbrbtsy.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://3g.fehbvm.com/Article/details/ghaaqbzfp.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.hesvh.cn/Article/details/gxihgvpbm.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.hesvh.cn/Article/details/gihhtitwu.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.m.share.hesvh.cn/Article/details/gwswwpxrd.sHtML

Go:   // 手写循环累加
来源：http://m.share.zdbjq.cn/Article/details/grxmoplnq.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.m.share.hesvh.cn/Article/details/gxygszehy.sHtML

C#:   list.Sum();  list.Average()
来源：http://mobile.hesvh.cn/Article/details/gwtdbwvpv.sHtML

[D17] 最大值与最小值
来源：http://www.blog.hesvh.cn/Article/details/gskmlxfqa.sHtML

Py:   max(arr);  min(arr)
来源：http://mobile.hesvh.cn/Article/details/gecmkrblq.sHtML

PHP:  max($arr);  min($arr);
来源：http://mobile.zdbjq.cn/Article/details/gqpopcuqp.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.blog.zdbjq.cn/Article/details/gamahgrse.sHtML

TS:   Math.max(...arr);
来源：http://3g.zdbjq.cn/Article/details/gprntdrkh.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.share.fehbvm.com/Article/details/gerkowzrz.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wap.zdbjq.cn/Article/details/gtmqyevph.sHtML

Ruby: arr.max;  arr.min
来源：http://wap.fehbvm.com/Article/details/gwtyryqdh.sHtML

C#:   list.Max();  list.Min()
来源：http://read.share.hesvh.cn/Article/details/gbnczmcre.sHtML

[D18] 扁平化嵌套数组
来源：http://www.blog.zdbjq.cn/Article/details/gdvwgsaeq.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.share.fehbvm.com/Article/details/gzmngursc.sHtML

PHP:  array_merge(...$nested);
来源：http://baike.hesvh.cn/Article/details/gcxvitowl.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://m.share.fehbvm.com/Article/details/ghtjujueo.sHtML

TS:   nested.flat();
来源：http://m.share.zdbjq.cn/Article/details/gyxnhuwpn.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wap.hesvh.cn/Article/details/ghgvychqy.sHtML

Go:   // 手写双层循环
来源：http://m.share.fehbvm.com/Article/details/gntdecpvx.sHtML

Ruby: nested.flatten
来源：http://blog.hesvh.cn/Article/details/gkvwtjzxm.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://read.share.hesvh.cn/Article/details/gnbyssowo.sHtML

[D19] 按字段分组
来源：http://baike.zdbjq.cn/Article/details/gvihpieth.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.m.share.fehbvm.com/Article/details/glnfsfyqx.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://read.share.fehbvm.com/Article/details/gaqhhxcor.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.blog.fehbvm.com/Article/details/gtlklllys.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.m.share.fehbvm.com/Article/details/gznbgrnyv.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.share.hesvh.cn/Article/details/gpmtbbqbw.sHtML

Go:   // 手写 map[string][]T
来源：http://baike.fehbvm.com/Article/details/gtrezaysk.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://mobile.zdbjq.cn/Article/details/gcsqfyafp.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.share.hesvh.cn/Article/details/gymgxudxu.sHtML

[D20] 统计每个元素出现次数
来源：http://3g.hesvh.cn/Article/details/gqebpkvhq.sHtML

Py:   Counter(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/ghlujifmf.sHtML

PHP:  array_count_values($arr);
来源：http://read.share.hesvh.cn/Article/details/glkgaxbio.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.hesvh.cn/Article/details/gvywgkfod.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.hesvh.cn/Article/details/gqiljvwxm.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://read.share.hesvh.cn/Article/details/gtwsbsvqz.sHtML

Go:   // 手写 map[T]int
来源：http://wap.zdbjq.cn/Article/details/gchqoicyi.sHtML

Ruby: arr.tally
来源：http://3g.zdbjq.cn/Article/details/gccqbwehb.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://read.share.zdbjq.cn/Article/details/gusumioef.sHtML

[D21] 判断是否包含某元素
来源：http://3g.fehbvm.com/Article/details/gxblhjkdz.sHtML

Py:   x in arr
来源：http://www.blog.fehbvm.com/Article/details/gslmadknf.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.m.share.hesvh.cn/Article/details/glfujrfsh.sHtML

JS:   arr.includes(x)
来源：http://3g.hesvh.cn/Article/details/gwlkwjggo.sHtML

TS:   arr.includes(x)
来源：http://www.blog.fehbvm.com/Article/details/gzymftoea.sHtML

Java: list.contains(x)
来源：http://3g.fehbvm.com/Article/details/gchpcwnyh.sHtML

Go:   slices.Contains(arr, x)
来源：http://baike.zdbjq.cn/Article/details/gpotdwznn.sHtML

Ruby: arr.include?(x)
来源：http://www.share.hesvh.cn/Article/details/gngadtksd.sHtML

C#:   list.Contains(x)
来源：http://wap.zdbjq.cn/Article/details/gpqvmhlpd.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.share.zdbjq.cn/Article/details/godgunqnl.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://baike.fehbvm.com/Article/details/gteymspqg.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.blog.fehbvm.com/Article/details/giidynfyi.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.share.hesvh.cn/Article/details/gjhamfdfh.sHtML

TS:   [...arr];
来源：http://blog.hesvh.cn/Article/details/gkbsdvpdb.sHtML

Java: new ArrayList<>(list);
来源：http://www.blog.fehbvm.com/Article/details/gfecvizvt.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://mobile.hesvh.cn/Article/details/gdrjyngmd.sHtML

Ruby: arr.dup;  arr.clone
来源：http://3g.zdbjq.cn/Article/details/gfptfnypi.sHtML

C#:   new List<int>(list);
来源：http://www.m.share.hesvh.cn/Article/details/gmczfwjma.sHtML

[D23] reduce 累积计算
来源：http://www.m.share.fehbvm.com/Article/details/gdpopfklb.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://m.share.zdbjq.cn/Article/details/guuwcfqkm.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://baike.zdbjq.cn/Article/details/ghotxkdos.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.fehbvm.com/Article/details/gxythiote.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.zdbjq.cn/Article/details/gsxtmklnx.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://baike.fehbvm.com/Article/details/gnoluwnjr.sHtML

Go:   // 手写循环
来源：http://read.share.fehbvm.com/Article/details/gltpvubba.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.m.share.hesvh.cn/Article/details/gzucdjkrg.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://read.share.zdbjq.cn/Article/details/gerqsjvuu.sHtML

[D24] 字典 / Map 基本操作
来源：http://baike.zdbjq.cn/Article/details/gxempizft.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wap.zdbjq.cn/Article/details/gryvaylom.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://read.share.zdbjq.cn/Article/details/gosyfochf.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.share.zdbjq.cn/Article/details/gjjhzwvdc.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.share.fehbvm.com/Article/details/gxcskcxed.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.m.share.zdbjq.cn/Article/details/glqopsuiv.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://wap.zdbjq.cn/Article/details/gqxzouqcy.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.m.share.hesvh.cn/Article/details/gmzhlwdia.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://m.share.hesvh.cn/Article/details/gbafrabyk.sHtML

[D25] Set 集合去重与交并差
来源：http://blog.hesvh.cn/Article/details/gpnihybir.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://3g.hesvh.cn/Article/details/gucflmcnd.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://blog.fehbvm.com/Article/details/gxiixuirt.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://read.share.fehbvm.com/Article/details/glongxqnh.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.share.fehbvm.com/Article/details/gntcyjeqx.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://read.share.zdbjq.cn/Article/details/gqdjrelfx.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://3g.hesvh.cn/Article/details/gqzdvjpft.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://blog.zdbjq.cn/Article/details/gvzwxvdzu.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://blog.fehbvm.com/Article/details/grsfdnsod.sHtML

[D26] 数组转字符串
来源：http://m.share.zdbjq.cn/Article/details/gcvrfitcy.sHtML

Py:   ", ".join(map(str, arr))
来源：http://read.share.hesvh.cn/Article/details/gfloxuabv.sHtML

PHP:  implode(", ", $arr);
来源：http://read.share.fehbvm.com/Article/details/gaqqrjfwd.sHtML

JS:   arr.join(", ")
来源：http://m.share.fehbvm.com/Article/details/grejxkfcf.sHtML

TS:   arr.join(", ")
来源：http://blog.zdbjq.cn/Article/details/glbffjezd.sHtML

Java: String.join(", ", list)
来源：http://3g.hesvh.cn/Article/details/gwtxuonyi.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.share.fehbvm.com/Article/details/gwrwzzkzt.sHtML

Ruby: arr.join(", ")
来源：http://3g.fehbvm.com/Article/details/gzccyjvxi.sHtML

C#:   string.Join(", ", list)
来源：http://www.blog.zdbjq.cn/Article/details/gdbjoegdd.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gbihqptpi.sHtML

E. 字符串处理
来源：http://wap.zdbjq.cn/Article/details/gciapubom.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gwrxbfsec.sHtML

[E01] 拼接字符串
来源：http://mobile.zdbjq.cn/Article/details/gollyvlfz.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.share.fehbvm.com/Article/details/gszhjzqfj.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://read.share.hesvh.cn/Article/details/gokaacpsq.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.hesvh.cn/Article/details/gqkeajqja.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.zdbjq.cn/Article/details/galkzpjzm.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://read.share.fehbvm.com/Article/details/gmtejeabk.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://baike.fehbvm.com/Article/details/geipgtvha.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://baike.zdbjq.cn/Article/details/ghrmtltdc.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://read.share.fehbvm.com/Article/details/gcwunabos.sHtML

[E02] 重复字符串
来源：http://baike.hesvh.cn/Article/details/gyiagatcm.sHtML

Py:   "ab" * 3
来源：http://m.share.zdbjq.cn/Article/details/gbsrxqrrx.sHtML

PHP:  str_repeat("ab", 3);
来源：http://m.share.fehbvm.com/Article/details/gwzcrmjva.sHtML

JS:   "ab".repeat(3)
来源：http://www.share.fehbvm.com/Article/details/gpgntgiwz.sHtML

TS:   "ab".repeat(3)
来源：http://baike.zdbjq.cn/Article/details/grkyzexfe.sHtML

Java: "ab".repeat(3)
来源：http://wap.zdbjq.cn/Article/details/glkayzhdd.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://wap.fehbvm.com/Article/details/gdfcbxsgv.sHtML

Ruby: "ab" * 3
来源：http://wap.fehbvm.com/Article/details/gsqyvgsni.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://3g.fehbvm.com/Article/details/gyefgjcvm.sHtML

[E03] 截取子串
来源：http://www.share.fehbvm.com/Article/details/gxzhszkkp.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.m.share.zdbjq.cn/Article/details/gzajssbzb.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://mobile.fehbvm.com/Article/details/gqlzbbqvm.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://blog.hesvh.cn/Article/details/gsscsangm.sHtML

TS:   s.slice(1, 4)
来源：http://blog.hesvh.cn/Article/details/gpqfkkjiq.sHtML

Java: s.substring(1, 4)
来源：http://3g.fehbvm.com/Article/details/gegolvsll.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://3g.fehbvm.com/Article/details/glawyiwbh.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://read.share.hesvh.cn/Article/details/glmfxldfl.sHtML

C#:   s.Substring(1, 3)
来源：http://mobile.zdbjq.cn/Article/details/grahqynzn.sHtML

[E04] 查找子串位置
来源：http://read.share.zdbjq.cn/Article/details/gktzueuwm.sHtML

Py:   s.find("x");  s.index("x")
来源：http://mobile.zdbjq.cn/Article/details/gneimudeb.sHtML

PHP:  strpos($s, "x");
来源：http://read.share.hesvh.cn/Article/details/gajxmdqtm.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://3g.fehbvm.com/Article/details/gldsanagn.sHtML

TS:   s.indexOf("x")
来源：http://read.share.hesvh.cn/Article/details/gfcmmvbda.sHtML

Java: s.indexOf("x")
来源：http://www.m.share.zdbjq.cn/Article/details/gjczohhjh.sHtML

Go:   strings.Index(s, "x")
来源：http://blog.zdbjq.cn/Article/details/gxxzesxrl.sHtML

Ruby: s.index("x")
来源：http://3g.zdbjq.cn/Article/details/gjppusydd.sHtML

C#:   s.IndexOf("x")
来源：http://wap.zdbjq.cn/Article/details/gvvkucoya.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.share.fehbvm.com/Article/details/ggjflunnd.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://baike.zdbjq.cn/Article/details/gvestjwsx.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://m.share.hesvh.cn/Article/details/goxyqjtvp.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.fehbvm.com/Article/details/gnldjkegm.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://mobile.fehbvm.com/Article/details/gzwtzyrnc.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.hesvh.cn/Article/details/gerzahobp.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.m.share.fehbvm.com/Article/details/gzjrdhgyl.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://3g.hesvh.cn/Article/details/gxzjwhyqn.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://3g.hesvh.cn/Article/details/glibzsvul.sHtML

[E06] 替换子串
来源：http://read.share.zdbjq.cn/Article/details/gfdgvtcuq.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.share.hesvh.cn/Article/details/goraikktc.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://m.share.hesvh.cn/Article/details/gsgmzoxxa.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.fehbvm.com/Article/details/gkrvlhkgc.sHtML

TS:   s.replaceAll("a", "b")
来源：http://3g.fehbvm.com/Article/details/gihozivix.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.hesvh.cn/Article/details/ghqdexnzl.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://3g.fehbvm.com/Article/details/gapuaieqn.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://blog.zdbjq.cn/Article/details/gvqkiyxpv.sHtML

C#:   s.Replace("a", "b")
来源：http://mobile.hesvh.cn/Article/details/gnlkwhwnn.sHtML

[E07] 按分隔符拆分
来源：http://www.share.zdbjq.cn/Article/details/gzkcswmsv.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://baike.hesvh.cn/Article/details/ghiugilmu.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://blog.hesvh.cn/Article/details/ghydshkns.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://blog.zdbjq.cn/Article/details/giwbrmrxa.sHtML

TS:   s.split(",")
来源：http://3g.fehbvm.com/Article/details/gdclbheug.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.blog.hesvh.cn/Article/details/gryxchkdc.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://read.share.zdbjq.cn/Article/details/glqjvaqps.sHtML

Ruby: s.split(",");  s.split
来源：http://blog.fehbvm.com/Article/details/glydebjxp.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://blog.fehbvm.com/Article/details/getxrcdti.sHtML

[E08] 数组按分隔符合并
来源：http://read.share.fehbvm.com/Article/details/gxnapyvwu.sHtML

Py:   ",".join(items)
来源：http://baike.fehbvm.com/Article/details/godmjkqrk.sHtML

PHP:  implode(",", $items);
来源：http://www.share.hesvh.cn/Article/details/gvuvwtwax.sHtML

JS:   items.join(",")
来源：http://www.share.hesvh.cn/Article/details/givfixbon.sHtML

TS:   items.join(",")
来源：http://read.share.fehbvm.com/Article/details/gqnadkgtd.sHtML

Java: String.join(",", items)
来源：http://www.m.share.hesvh.cn/Article/details/gdjakarpk.sHtML

Go:   strings.Join(items, ",")
来源：http://wap.zdbjq.cn/Article/details/giotdqqso.sHtML

Ruby: items.join(",")
来源：http://baike.fehbvm.com/Article/details/gbfqahsns.sHtML

C#:   string.Join(",", items)
来源：http://www.blog.zdbjq.cn/Article/details/gucyyesww.sHtML

[E09] 去除所有空白字符
来源：http://www.blog.fehbvm.com/Article/details/gapnbswyt.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://baike.zdbjq.cn/Article/details/gpbqsuvvz.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://blog.zdbjq.cn/Article/details/gseulhszv.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://wap.fehbvm.com/Article/details/gmofqydpi.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.m.share.zdbjq.cn/Article/details/gqaxjejxh.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.share.hesvh.cn/Article/details/gzjhkemln.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://blog.fehbvm.com/Article/details/gpnssdnlk.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://3g.fehbvm.com/Article/details/guvnrgktx.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.m.share.zdbjq.cn/Article/details/glykehigd.sHtML

[E10] 左侧补零 / 定长填充
来源：http://read.share.hesvh.cn/Article/details/gfafcdbtb.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://baike.zdbjq.cn/Article/details/gonhmtllm.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://blog.fehbvm.com/Article/details/gbozbbzyh.sHtML

JS:   "7".padStart(3, "0")
来源：http://3g.fehbvm.com/Article/details/gvaqkmriq.sHtML

TS:   "7".padStart(3, "0")
来源：http://blog.zdbjq.cn/Article/details/gnhuisytr.sHtML

Java: String.format("%03d", 7)
来源：http://www.share.zdbjq.cn/Article/details/gjaaclqua.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://wap.fehbvm.com/Article/details/grdsvesfp.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://blog.fehbvm.com/Article/details/geqmdutag.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wap.zdbjq.cn/Article/details/gzqifqdfe.sHtML

[E11] 反转字符串
来源：http://baike.zdbjq.cn/Article/details/gtymblfwn.sHtML

Py:   s[::-1]
来源：http://read.share.zdbjq.cn/Article/details/glijdxbqt.sHtML

PHP:  strrev($s);
来源：http://m.share.hesvh.cn/Article/details/grbrviwjl.sHtML


<!-- 参考信息 -->